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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Kixie is a Los Angeles based sales-engagement and revenue-communications platform built around
PowerCall — a multi-line power dialer, business phone service and SMS/MMS product with
bi-directional CRM integrations. Its public API is a small, event-oriented HTTP surface on the
`apig.kixie.com` gateway.

- Website: https://www.kixie.com/
- Developer portal: https://developer.kixie.com/
- Status: https://status.kixie.com/

## What Kixie publishes

| Surface | Base | Notes |
|---|---|---|
| Kixie Event API | `https://apig.kixie.com/app/event` | One POST endpoint dispatching on an `eventname` string — calls, SMS, Team SMS, queues, cadences, PowerLists |
| Kixie Webhook Management API | `https://apig.kixie.com/app/v1/api` | Create / update / list / delete the eight documented event webhooks |
| Kixie Agent Status API | `https://apig.kixie.com/www/agent/status` | The only read-only operation in the public surface |

Nine webhook event types are documented with full payload examples, plus four inbound "Custom CRM"
callbacks that Kixie invokes against customer-operated endpoints.

## Not published by Kixie

Recorded so that absence reads as deliberate rather than as something we failed to find. Every item
below was probed on 2026-08-12; see `well-known/kixie-well-known.yml` for URLs and status codes.

- **No machine-readable contract** — no OpenAPI, Swagger, AsyncAPI, GraphQL SDL or JSON Schema on
  any host. The reference is server-rendered HTML.
- **No client SDKs** — npm, PyPI, RubyGems, NuGet, crates.io and Packagist all return zero
  first-party packages. Neither repo in the `Kixie-com` GitHub org is an API client.
- **No CLI, no MCP server, no A2A agent card, no `/.well-known/` documents of any kind.**
- **No idempotency support** on operations that place calls and send SMS.
- **No error catalogue** and no documented rate-limit response headers (the 10,000/day account
  quota is published in prose, in one help-center article).
- **No deprecation policy, no SLA, no public roadmap**, and no published prices for any of the
  three subscription tiers.
- **No compliance certifications** — and Kixie says so on purpose: its security page
  "intentionally does not claim a certification, audit result, hosting architecture, retention
  period, or control that has not been confirmed for publication."

Kixie does run a public Atlassian Statuspage with an open JSON API that tracks named API endpoints
as individual components, and publishes a security contact with reporting instructions at
https://www.kixie.com/security/.

> **Note on probing this domain.** `www.kixie.com` and `developer.kixie.com` run WordPress with
> fuzzy-match URL redirection: unknown paths return `301` to a loosely-similar marketing page
> rather than `404`. `/.well-known/agent-card.json` redirects to `/integrations/agentforce-marketing/`
> and `/roadmap/` redirects to `/integrations/monday/`. A crawler that follows redirects and records
> the final `200` will falsely credit Kixie with documents it does not serve. Verify the body.
