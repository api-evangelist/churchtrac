# ChurchTrac

ChurchTrac is all-in-one church management software (ChMS) headquartered in
Jacksonville, Florida, founded in 2003 by Byron Tedder. It serves small and large
churches with people/member management, church directory, groups, attendance and
check-in, event registration, worship planning and volunteer scheduling, online
giving, and fund accounting/budgeting. Website: https://www.churchtrac.com/

## API Access Model — Honest Stub (No Public API)

**ChurchTrac does not publish a public or partner developer API.** As of this
review (2026-07-03), there is:

- **No documented REST API**, base URL, or API reference for ChurchTrac data.
- **No API keys, OAuth, or personal access tokens** for third-party developers.
- **No documented webhooks** or event/streaming surface (no WebSocket, no SSE).
- **No Zapier/Make integration** published by ChurchTrac.

What ChurchTrac markets as "integrations" are **ChurchTrac consuming other
providers' APIs on the church's behalf**, not an API that ChurchTrac exposes:

- **Stripe** — payment processing for online giving.
- **SendGrid / Mailchimp / Constant Contact** — email delivery and list sync.
- **Twilio** — church texting / enhanced messaging.
- **QuickBooks Online** — accounting export/sync.
- **Zoom, Microsoft Outlook** — meetings and calendar.

Member- and public-facing access is delivered through the **Church Connect** app
(a member portal / mobile experience) and **embeddable online giving forms**
(iframe/embed snippet you place on a church website) — neither is a programmable
API for reading or writing ChurchTrac records.

This entry is intentionally a stub. No `openapi/`, `plans/`, `rate-limits/`,
`finops/`, or `collections/` artifacts were fabricated because no sourced API,
rate-limit, or programmatic-billing details exist to model. If ChurchTrac ships a
documented developer API in the future, this repo should be upgraded from stub to
a full APIs.json 0.19+ catalog with real `apis` entries and an OpenAPI document.

For comparison, several competing ChMS platforms *do* offer public/partner APIs
(ChurchTools, ChurchSuite, Fellowship One, Planning Center), which is why the
absence of one here is documented explicitly rather than assumed.

## Pricing

ChurchTrac pricing starts at roughly **$9/month** and is tiered by the number of
people ("names") you track — plan tiers around 75, 125, 250, 500, 1,000, and
unlimited names — plus optional add-ons (Enhanced Messaging/texting credits,
accounting service). A free trial is available. See
https://www.churchtrac.com/pricing for current tiers. Note: this is
**subscription pricing for the software product**, not API/usage-metered pricing,
because there is no API to meter.

## Files

- `apis.yml` — APIs.json 0.19 provider descriptor (company-level; no `apis`
  collection because there is no public API).
- `review.yml` — API Evangelist review answering whether ChurchTrac exposes a
  documented public WebSocket API (it does not; it exposes no public API at all).
- `README.md` — this file.

## Sources

- https://www.churchtrac.com/ — product homepage and feature set.
- https://www.churchtrac.com/support — support/help center (no developer API docs).
- https://www.churchtrac.com/support/connect — Church Connect member app.
- https://www.churchtrac.com/pricing — per-names subscription tiers.
- https://www.linkedin.com/company/churchtrac — company profile (Jacksonville, FL).
