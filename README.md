# Kixie

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

Kixie is a Los Angeles based sales-engagement and revenue-communications platform built around PowerCall, a multi-line power dialer, business phone service and SMS/MMS product that plugs bi-directionally into HubSpot, Salesforce, Pipedrive, Zoho and GoHighLevel. Its public developer surface is a small, event-oriented HTTP API served from the apig.kixie.com gateway: a single POST /app/event endpoint that dispatches on an eventname discriminator to place calls, send SMS and Team SMS, add and remove contacts from PowerLists, push numbers into and out of calling queues and cadences; a webhook management API for creating, listing, updating and deleting the eight documented event webhooks; and an agent-status lookup. Authentication is a single account scoped API key plus a Business ID, and the platform publishes a documented daily usage cap of 10,000 API calls per account. Kixie publishes no OpenAPI, AsyncAPI or GraphQL contract and ships no first-party client SDKs; the reference is human-readable HTML on developer.kixie.com and in the Zendesk help center.

**Areas:** Company · Sales Engagement · Voice · Telephony · SMS · Messaging · Contact Center · Power Dialer · CRM · Webhook · Communications · Revenue Operations

## Kixie on APIs.io

Everything profiled for Kixie is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/kixie/](https://apis.io/providers/kixie/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [Kixie Event API](https://apis.io/apis/kixie/kixie-event-api/) — The primary Kixie automation surface. A single POST endpoint on the apig.kixie.com gateway that dispatches on an `eventname` discriminator in the JSON body…
- [Kixie Webhook Management API](https://apis.io/apis/kixie/kixie-webhook-management-api/) — A path-versioned management surface for Kixie's event webhooks. Four POST operations — postWebhook (create), putWebhook (update), getWebhooks (list) and…
- [Kixie Agent Status API](https://apis.io/apis/kixie/kixie-agent-status-api/) — A read-only lookup that returns the current presence of a Kixie agent by email address — whether the agent's device is registered (logged in) and whether…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Kixie Webhooks](https://apis.io/asyncapis/kixie/kixie-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Kixie MCP server](https://apis.io/servers/kixie/kixie-mcp-server/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Kixie Authentication](https://apis.io/security/kixie/kixie-authentication/)
- [Kixie Domain Security](https://apis.io/security/kixie/kixie-domain-security/)
- [Kixie Trust Center](https://apis.io/security/kixie/kixie-trust-center/)
- [Kixie Vulnerability Disclosure](https://apis.io/security/kixie/kixie-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Kixie Plans Pricing](https://apis.io/plans/kixie/kixie-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Kixie Rate Limits](https://apis.io/rate-limits/kixie/kixie-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.kixie.com/)
- [Documentation](https://developer.kixie.com/)
- [Getting started](https://support.kixie.com/hc/en-us/articles/7273987300635-Kixie-Authentication-Overview)
- [API reference](https://developer.kixie.com/)
- [Pricing](https://www.kixie.com/pricing/)
- [Sign up](https://www.kixie.com/sign-up/)
- [Support](https://support.kixie.com/hc/en-us)
- [Blog](https://www.kixie.com/sales-blog/)
- [Terms of service](https://www.kixie.com/terms/)
- [Privacy policy](https://www.kixie.com/privacy/)
- [GitHub](https://github.com/Kixie-com)
- [Status](https://status.kixie.com/)

## API Evangelist rating

**Kin Score 57.6** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 39.0 |
| Contract governance | 18.2 |
| Operational transparency | 73.7 |
| Developer ergonomics | 59.5 |
| Access clarity | 73.7 |

**Agent readiness 22.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 35.8** — Telecommunications

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/kixie/](https://apis.io/providers/kixie/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Kixie: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/kixie/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
