---
name: Set up recurring billing with Malga subscriptions
description: Create and manage a recurring subscription (Malga recurrence engine), then handle lifecycle actions and webhook notifications.
api: openapi/plug-openapi-original.yml
operations: [createSubscription, getSubscription, updateSubscription, cancelSubscription, pauseSubscription, resumeSubscription, listSubscriptionCycles, createWebhook]
---

# Recurring billing with Malga

## Auth
`X-Client-Id` + `X-Api-Key` headers on every call. Base URL `https://api.malga.io`.

## Steps
1. **Create a subscription** — `createSubscription` (`POST /v1/subscriptions`) with the customer, payment method and schedule.
2. **Register a webhook** — `createWebhook` (`POST /v1/webhooks`) to receive recurrence events (status changes, new charges). Verify the HMAC signature on each delivery (see asyncapi/plug-webhooks.yml).
3. **Manage the lifecycle**:
   - Pause: `pauseSubscription` (`PATCH /v1/subscriptions/{id}/pause`)
   - Resume: `resumeSubscription` (`PATCH /v1/subscriptions/{id}/resume`)
   - Cancel: `cancelSubscription` (`PATCH /v1/subscriptions/{id}/cancel`)
   - Update: `updateSubscription` (`PUT /v1/subscriptions/{id}`)
4. **Inspect billing cycles** — `listSubscriptionCycles` (`GET /v1/subscriptions/{id}/cycles`) and `getSubscription` (`GET /v1/subscriptions/{id}`).

## Rules
- Use `X-Idempotency-Key` on the create call. See conventions/plug-conventions.yml.
- Handle declined recurring charges via `declinedCode` (errors/plug-decline-codes.yml).
