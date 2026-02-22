# apipick-public-holidays

A [Claude Code](https://claude.ai/claude-code) skill that retrieves public holidays for any country and year using the [apipick](https://www.apipick.com) Public Holidays API.

## What it does

Given a country (ISO 3166-1 alpha-2 code) and an optional year, this skill returns:

- **Holiday list** — all public holidays sorted by date
- **Holiday names** — official names in English
- **Total count** — number of public holidays in the year

Supports 100+ countries. Year range: 1900 to 10 years ahead.

## Requirements

An apipick API key is required. Get 100 free credits at [apipick.com](https://www.apipick.com).

## Installation

Install via Claude Code:

```bash
claude skills install https://github.com/apipick-lab/apipick-public-holidays
```

## Usage

Once installed, just ask Claude naturally:

- *"What are the public holidays in the US this year?"*
- *"List all public holidays in Japan for 2026"*
- *"Is December 26 a holiday in the UK?"*
- *"How many public holidays does Singapore have?"*

Claude will convert country names to ISO codes automatically and call the apipick API.

## API Reference

| Field | Value |
|-------|-------|
| Endpoint | `GET https://www.apipick.com/api/holidays` |
| Auth | `x-api-key` header |
| Cost | 1 credit per request |

See [`references/api_reference.md`](references/api_reference.md) for full documentation.

## Links

- [apipick.com](https://www.apipick.com) — API platform
- [Public Holidays](https://www.apipick.com/public-holidays) — product page
- [Get API Key](https://www.apipick.com/dashboard/api-keys)
