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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Stooq is a Poland-based financial data platform providing free historical and current market
data for global equities, indices, currencies, cryptocurrencies, commodities, bonds, and
economic indicators. Data is delivered as CSV via a simple REST-style URL interface.

## API

The primary endpoint is `https://stooq.com/q/d/l/` with query parameters:

| Parameter | Description |
|-----------|-------------|
| `s` | Ticker symbol with optional exchange suffix (e.g. `AAPL.US`, `VOD.UK`, `BMW.DE`) |
| `d1` | Start date in YYYYMMDD format |
| `d2` | End date in YYYYMMDD format |
| `i` | Interval: `d` daily, `w` weekly, `m` monthly, `q` quarterly, `y` yearly |
| `apikey` | API key obtained via on-site CAPTCHA (required as of early 2026) |

Response columns: Date, Open, High, Low, Close, Volume.

### Exchange Suffixes

`.US` NYSE/NASDAQ, `.UK` London SE, `.DE` Deutsche Borse, `.JP` Tokyo SE, `.HK` Hong Kong,
`.HU` Budapest SE. No suffix defaults to Warsaw Stock Exchange (GPW).

### Bulk Downloads

Point-in-time database snapshots (12,000+ securities, ZIP-compressed CSV) are available at
`https://stooq.com/db/h/` for daily, weekly, and monthly frequencies across multiple regions.

## Coverage

- 21,000+ global securities and ETFs
- 1,980+ currency pairs
- 130+ cryptocurrencies
- Global indices, commodities, bonds, economic indicators
- Daily history: 30+ years for major instruments
- Hourly history: ~9 months
- 5-minute history: ~1 month

## Rate Limits

A daily request quota is enforced per API key. The exact limit is not published. Exceeding
it returns an error message in the response body with HTTP 200. Implement response-body
checking and local caching to manage quota consumption.

## Links

- Portal: https://stooq.com/
- Bulk Data: https://stooq.com/db/h/
- API Key: https://stooq.com/q/d/?s=spy.us&get_apikey
