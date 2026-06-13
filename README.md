# Stooq

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
