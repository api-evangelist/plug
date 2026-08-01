---
name: Create a customer and charge a card with Malga
description: Tokenize a card, create a customer, and run an idempotent card charge through Malga's payment orchestration API, then capture or refund it.
api: openapi/plug-openapi-original.yml
operations: [create_token, createCustomer, saveCard, charge, captureCharge, refundCharge, getChargesByid]
---

# Create a customer and charge a card (Malga)

Malga (formerly Plug) is a Brazilian payment orchestration API. Base URL `https://api.malga.io`.

## Auth
Send both headers on every request (keys from the Malga dashboard):
- `X-Client-Id: <client id>`
- `X-Api-Key: <secret key>`

## Steps
1. **Tokenize the card** — `create_token` (`POST /v1/tokens`). Prefer client-side tokenization via `@malga/tokenization` so PAN never touches your server.
2. **Create a customer** — `createCustomer` (`POST /v1/customers`).
3. **(Optional) Save the card to the customer** — `saveCard` (`POST /v1/cards`) / `linkCard` (`POST /v1/customers/{customer_id}/cards`).
4. **Charge** — `charge` (`POST /v1/charges`) with the token or saved card as the payment source. Send a unique `X-Idempotency-Key` header so retries do not double-charge.
5. **Capture** a pre-authorized charge with `captureCharge` (`POST /v1/charges/{id}/capture`), or **refund/void** with `refundCharge` (`POST /v1/charges/{id}/void`).
6. **Confirm** — `getChargesByid` (`GET /v1/charges/{id}`).

## Rules
- Idempotency: all POST calls accept `X-Idempotency-Key` (client-generated, unique). Retry 3-5 times, >=10s apart. See conventions/plug-conventions.yml.
- On decline, read the `declinedCode` on the charge (see errors/plug-decline-codes.yml) — respect `retryable` before retrying.
- Test in sandbox: card outcome is driven by the final digit (0/1/4 approve, 2/3/5/6/7 decline). See sandbox/plug-sandbox.yml.
