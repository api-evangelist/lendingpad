# LendingPad (lendingpad)

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

LendingPad is a cloud-based mortgage loan origination system (LOS) that lets brokers, lenders, and institutions originate, process, underwrite, close, and fund residential mortgage loans with real-time, multi-user collaboration across the borrower, broker, lender, and service-provider lifecycle. It ships in Broker, Lender, Processing, and Institution editions and runs a large Partners Marketplace of integrated vendors (credit, AUS, AVM/appraisal, title, compliance, doc-prep, pricing/PPE, POS, CRM, and investors such as Fannie Mae, Freddie Mac, UWM, and Rocket Mortgage). Founded in 2015 and headquartered in McLean, Virginia.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/lendingpad/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/lendingpad/refs/heads/main/apis.yml)

## API access model — gated / partner-only

This entry is intentionally an **honest gated stub**. LendingPad does **not** publish a public, self-serve developer API. It exposes an **Enterprise API** for loan-data exchange, but per its [API Terms](https://lendingpad.com/api-terms):

- Access is limited to **Lender Edition** clients.
- An **executed API Agreement** and an **NDA** are required before evaluation/development.
- **API keys and testing-site access** are provisioned manually by the LendingPad support desk.
- Fees vary by **integration complexity**; dedicated support is billed at LendingPad's standard support rate.
- Import/export is throttled (reported ~30-minute intervals).
- LendingPad reserves the right to require a **qualified contractor** if a developer/vendor is deemed unqualified.

There is **no public developer portal, no public API reference, and no published endpoint list, base URL, or authentication spec.** Most integration happens through the curated [Partners Marketplace](https://lendingpad.com/partners-marketplace). Partner integrations describe MISMO-style 3.2/3.4 loan-data exchange into the LOS.

The API entries below are **modeled** from publicly described marketplace and partner-integration capabilities (flagged `endpointsModeled: true` in `apis.yml`). No endpoint-level surface, OpenAPI, or AsyncAPI has been fabricated.

## Tags

- Mortgage
- Loan Origination System
- LOS
- Lending
- FinTech
- Financial Services
- Real Estate
- Partner API
- Gated API

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs (modeled)

### LendingPad Loans API (modeled)

Loan-file exchange — create, read, and update mortgage loan files, submit loan data to lenders/investors, and import/export loan data (MISMO-style 3.2/3.4). No public endpoint reference; gated to Lender Edition under an executed API Agreement.

- **Human URL:** [https://lendingpad.com/partners-marketplace](https://lendingpad.com/partners-marketplace)

### LendingPad Documents & Conditions API (modeled)

Document and condition exchange — push borrower/loan documents into the LOS (as Floify and DocMagic do) and manage underwriting conditions, disclosures, and eSign. Publicly described as a partner capability; no documented endpoints.

- **Human URL:** [https://lendingpad.com/partners-marketplace](https://lendingpad.com/partners-marketplace)

### LendingPad Pricing & Product Eligibility API (modeled)

Product, pricing, and eligibility (PPE) exchange — integrations with pricing engines such as Polly, Lender Price, Optimal Blue, and LoanNex return real-time product/pricing results into the loan file. Delivered as marketplace integrations rather than a public developer API.

- **Human URL:** [https://lendingpad.com/partners-marketplace](https://lendingpad.com/partners-marketplace)

### LendingPad Webhooks & Events (modeled)

Event/notification surface — partner integrations describe synchronization of field updates, critical dates, and loan-status changes back to external systems (e.g. Shape's bi-directional sync). No public webhook/event reference is documented.

- **Human URL:** [https://lendingpad.com/partners-marketplace](https://lendingpad.com/partners-marketplace)

## Common Properties

- [Website](https://lendingpad.com)
- [LinkedIn](https://www.linkedin.com/company/lendingpad)
- [Documentation (API Terms)](https://lendingpad.com/api-terms)
- [Partner Program](https://lendingpad.com/partners-marketplace)
- [Knowledge Base](https://kb.lendingpad.com/integrations)
- [Blog](https://blog.lendingpad.com)
- [Plans](plans/lendingpad-plans-pricing.yml)

## Plans & Pricing

LendingPad does not publish an official price list. Indicative, third-party-reported pricing by edition:

- **Broker Edition:** ~$40–$55 per user/month (some sources up to $100); core LOS, compliance, POS, wholesale integration.
- **Lender Edition:** ~$100–$200 per closed loan (success-linked); unlimited users, secondary/funding/post-closing, **Enterprise API access** (gated).
- **Processing Edition:** quote on request; back-office roles and multi-client pipelines.
- **Institution Edition:** quote on request; all features, full network access, all channels.

See [`plans/lendingpad-plans-pricing.yml`](plans/lendingpad-plans-pricing.yml). API access is not sold as a self-serve product.

## Review

Does LendingPad expose a documented public WebSocket API? **No.** See [`review.yml`](review.yml). LendingPad publishes no public API reference at all — and specifically no WebSocket or server-push transport.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
