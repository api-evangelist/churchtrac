# ChurchTrac

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
