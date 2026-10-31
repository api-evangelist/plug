# Malga

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Malga (formerly Plug / plugpagamentos.com) is a Brazilian intelligent payment infrastructure and orchestration platform. It lets companies route transactions across multiple acquirers, payment providers, methods (card, Pix, boleto, wallets such as PicPay and Apple Pay) and anti-fraud engines from a single API, with smart routing/retry flows, tokenization, 3D Secure 2, subscriptions/recurrence, split payments, sellers/payouts and a GraphQL analytics API. Malga is PCI DSS Level 1 compliant and backed by Lightspeed Venture Partners and QED Investors.

**Areas:** Company · Payments · Payment Orchestration · Payment Gateway · Fintech · Pix · Tokenization · Subscription · Brazil

## Malga on APIs.io

Everything profiled for Malga is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/plug/](https://apis.io/providers/plug/)** — or go straight to one of the APIs or properties below.

### APIs (19)

- [Malga Analytics API](https://apis.io/apis/plug/malga-analytics-api/) — GraphQL API for querying processed payment data (charges, cards, authorization rates).
- [Malga 3DS2 Malga API](https://apis.io/apis/plug/plug-3ds2-malga-api/) — The 3DS2 Malga API from Malga — 1 operation(s) for 3ds2 malga.
- [Malga Cards API](https://apis.io/apis/plug/plug-cards-api/) — **Dados básicos de um objeto cartão** <SchemaDefinition schemaRef="#/components/schemas/Card" />
- [Malga Charges API](https://apis.io/apis/plug/plug-charges-api/) — Para realizar uma cobrança deve criar um objeto `charge`. É possível recuperar detalhes de transações individuais ou listar todas as cobranças realizadas em…
- [Malga Client-token API](https://apis.io/apis/plug/plug-client-token-api/) — É possível criar chaves públicas de acesso temporária a API com escopo e tempo de expiração limitados. Recomendamos o uso deste tipo de chave quando você…
- [Malga Customers API](https://apis.io/apis/plug/plug-customers-api/) — Através da API de `customers` é possível realizar a criação, edição, listagem e exclusão de dados de compradores para uso nos serviços de tokenização de…
- [Malga Flows API](https://apis.io/apis/plug/plug-flows-api/) — Através da API de `flows` é possível recuperar detalhes de um Fluxo ou listar todas os Fluxos cadastrados em determinado `clientId`. Os fluxos inteligentes…
- [Malga Merchants API](https://apis.io/apis/plug/plug-merchants-api/) — Através das APIs de `merchants` é possível realizar a criação e configuração de sub contas na Malga. Uma sub conta, ou um `merchant`, é um cadastro de…
- [Malga Payouts API](https://apis.io/apis/plug/plug-payouts-api/) — Através das APIs de `payouts` é possível consultar o saldo disponível, listar repasses e visualizar as ordens de pagamento liquidadas para um cliente. Esses…
- [Malga Prepayment API](https://apis.io/apis/plug/plug-prepayment-api/) — > **🚧 Beta** — esta API está em fase Beta. Já está disponível para clientes habilitados, mas detalhes do contrato e do fluxo podem evoluir nas próximas…
- [Malga Providers API](https://apis.io/apis/plug/plug-providers-api/) — Através das APIs de Providers você pode realizar a edição e atualização dos provedores vinculados a um merchant já cadastrado na Malga. Essas operações…
- [Malga Seller Documents API](https://apis.io/apis/plug/plug-seller-documents-api/) — The Seller Documents API from Malga — 2 operation(s) for seller documents.
- [Malga Sellers API](https://apis.io/apis/plug/plug-sellers-api/) — Para realizar uma cobrança com Split, antes é necessário criar um `seller`. Os `sellers` são identificados a partir de um id único. Através das APIs de…
- [Malga Sessions API](https://apis.io/apis/plug/plug-sessions-api/) — Através da API de sessões é possível criar um pedido, composto por itens, métodos de pagamento e outros atributos, que pode ser pago através de um endpoint…
- [Malga Settings API](https://apis.io/apis/plug/plug-settings-api/) — Através da API de `settings` é possível recuperar, criar e atualizar configurações de personalização de link de pagamento de um determinado `clientId`. É…
- [Malga Subscriptions API](https://apis.io/apis/plug/plug-subscriptions-api/) — Através da API de `subscriptions` é possível realizar a criação, edição, listagem e exclusão de assinaturas. **Dados básicos de um objeto do tipo…
- [Malga Tokens API](https://apis.io/apis/plug/plug-tokens-api/) — **Dados básicos de uma requisição de criação de card token** <SchemaDefinition schemaRef="#/components/schemas/TokenRequest" />
- [Malga Vendors API](https://apis.io/apis/plug/plug-vendors-api/) — The Vendors API from Malga — 2 operation(s) for vendors.
- [Malga Webhooks API](https://apis.io/apis/plug/plug-webhooks-api/) — A Malga utiliza o serviço de webhooks para notificar o seu sistema sobre os eventos ocorridos na nossa plataforma. Através de webhooks você consegue…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Plug Webhooks](https://apis.io/asyncapis/plug/plug-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [malga](https://apis.io/servers/plug/malga/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Plug Agentic Access](https://apis.io/agentic-access/plug/plug-agentic-access/)

#### Collections (18)

Postman and Open Collection request collections.

- [Documentação Malga 3DS2 Malga API](https://apis.io/collections/plug/open-plug-3ds2-malga-api/)
- [Documentação Malga 3DS2 Malga Cards API](https://apis.io/collections/plug/open-plug-cards-api/)
- [Documentação Malga 3DS2 Malga Charges API](https://apis.io/collections/plug/open-plug-charges-api/)
- [Documentação Malga 3DS2 Malga Client-token API](https://apis.io/collections/plug/open-plug-client-token-api/)
- [Documentação Malga 3DS2 Malga Customers API](https://apis.io/collections/plug/open-plug-customers-api/)
- [Documentação Malga 3DS2 Malga Flows API](https://apis.io/collections/plug/open-plug-flows-api/)
- [Documentação Malga 3DS2 Malga Merchants API](https://apis.io/collections/plug/open-plug-merchants-api/)
- [Documentação Malga 3DS2 Malga Payouts API](https://apis.io/collections/plug/open-plug-payouts-api/)
- [Documentação Malga 3DS2 Malga Prepayment API](https://apis.io/collections/plug/open-plug-prepayment-api/)
- [Documentação Malga 3DS2 Malga Providers API](https://apis.io/collections/plug/open-plug-providers-api/)
- [Documentação Malga 3DS2 Malga Seller Documents API](https://apis.io/collections/plug/open-plug-seller-documents-api/)
- [Documentação Malga 3DS2 Malga Sellers API](https://apis.io/collections/plug/open-plug-sellers-api/)
- [Documentação Malga 3DS2 Malga Sessions API](https://apis.io/collections/plug/open-plug-sessions-api/)
- [Documentação Malga 3DS2 Malga Settings API](https://apis.io/collections/plug/open-plug-settings-api/)
- [Documentação Malga 3DS2 Malga Subscriptions API](https://apis.io/collections/plug/open-plug-subscriptions-api/)
- [Documentação Malga 3DS2 Malga Tokens API](https://apis.io/collections/plug/open-plug-tokens-api/)
- [Documentação Malga 3DS2 Malga Vendors API](https://apis.io/collections/plug/open-plug-vendors-api/)
- [Documentação Malga 3DS2 Malga Webhooks API](https://apis.io/collections/plug/open-plug-webhooks-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Plug Openapi Overlay](https://apis.io/overlays/plug/plug-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Plug Authentication](https://apis.io/security/plug/plug-authentication/)
- [Plug Domain Security](https://apis.io/security/plug/plug-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://malga.io/)
- [Documentation](https://docs.malga.io/documentations/welcome/introduction)
- [Getting started](https://docs.malga.io/documentations/welcome/introduction)
- [API reference](https://docs.malga.io/api-reference/about-apis)
- [Sign up](https://dashboard.malga.io/)
- [Changelog](https://docs.malga.io/release-notes)
- [Blog](https://malga.io/blog/)
- [GitHub](https://github.com/plughacker)
- [Status](https://status.malga.io/)

## API Evangelist rating

**Kin Score 47.2** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 59.4 |
| Contract governance | 18.2 |
| Operational transparency | 50.0 |
| Developer ergonomics | 73.2 |
| Access clarity | 7.9 |

**Agent readiness 39.9** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 25.0** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/plug/](https://apis.io/providers/plug/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Malga: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/plug/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
