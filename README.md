# Stooq

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

Stooq is a Poland-based financial data platform offering free access to historical and current market data for global equities, indices, currencies, cryptocurrencies, commodities, bonds, and economic indicators. Data is delivered as CSV via a simple REST-style URL interface at https://stooq.com/q/d/l/ using query parameters for ticker symbol, date range, and interval. As of early 2026 an API key (obtained via CAPTCHA on the site) is required. A known daily request quota applies; exceeding it returns an "Exceeded the daily hits limit" message. Bulk point-in-time snapshots of the full database (12,000+ securities) are also available as ZIP-compressed CSVs from https://stooq.com/db/h/.

**Areas:** Fintech · Market Data · Stocks · Indices · Currency · Cryptocurrency · Commodities · Historical Data · Free

## Stooq on APIs.io

Everything profiled for Stooq is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/stooq/](https://apis.io/providers/stooq/)** — or go straight to one of the APIs or properties below.

### APIs (1)

- [Stooq Q API](https://apis.io/apis/stooq/stooq-q-api/) — The Q API from Stooq — 1 operation(s) for q.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Stooq Agentic Access](https://apis.io/agentic-access/stooq/stooq-agentic-access/)

#### JSON Schema (2)

The data models the API reads and writes.

- [Stooq OHLCV Record](https://apis.io/schemas/stooq/stooq-ohlcv-record/)
- [Stooq Historical Data API Query Parameters](https://apis.io/schemas/stooq/stooq-query-parameters/)

#### Examples (3)

Example requests and responses.

- [Stooq Apple Daily Ohlcv Example](https://apis.io/examples/stooq/stooq-apple-daily-ohlcv-example/)
- [Stooq Bitcoin Weekly Ohlcv Example](https://apis.io/examples/stooq/stooq-bitcoin-weekly-ohlcv-example/)
- [Stooq Quota Exceeded Example](https://apis.io/examples/stooq/stooq-quota-exceeded-example/)

#### Collections (1)

Postman and Open Collection request collections.

- [Stooq Historical Data Q API](https://apis.io/collections/stooq/open-stooq-q-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Stooq — jsonschema rules](https://apis.io/rules/stooq/stooq-jsonschema-spectral-rules/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Stooq Domain Security](https://apis.io/security/stooq/stooq-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Stooq Plans Pricing](https://apis.io/plans/stooq/stooq-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Stooq Rate Limits](https://apis.io/rate-limits/stooq/stooq-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Stooq Finops](https://apis.io/finops/stooq/stooq-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.stooq.com/)
- [Documentation](https://stooq.com/db/h/)

## API Evangelist rating

**Kin Score 28.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 57.2 |
| Contract governance | 23.5 |
| Operational transparency | 5.3 |
| Developer ergonomics | 19.0 |
| Access clarity | 5.3 |

**Agent readiness 23.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 15.7** — Securities & Market Data

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/stooq/](https://apis.io/providers/stooq/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Stooq: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/stooq/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
