# Changelog

## 1.1.0 — Public skeleton
- Replaced inline secrets with env vars:
  - `X-Api-Key` → `={{ $env.INDUSTRY_NEWSAPI_KEY }}`
  - Google Sheets `documentId` → `={{ $env.INDUSTRY_SHEET_ID }}`
  - Email `fromEmail` → `={{ $env.INDUSTRY_FROM_EMAIL }}`
- Added **Format Data** node that renders compact HTML for email clients.
- Kept updated Gemini prompt that outputs STRICT JSON for the formatter.

## 1.0.0 — Private build
- Weekly schedule → fetch news → Gemini analysis → email digest to leadership.
