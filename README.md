# LendingPad

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

LendingPad is a cloud-based mortgage loan origination system (LOS) that lets brokers, lenders, and institutions originate, process, underwrite, close, and fund residential mortgage loans with real-time, multi-user collaboration across the borrower, broker, lender, and service-provider lifecycle. It ships in Broker, Lender, Processing, and Institution editions and runs a large Partners Marketplace of integrated vendors (credit, AUS, AVM/appraisal, title, compliance, doc-prep, pricing/PPE, POS, CRM, and investors such as Fannie Mae, Freddie Mac, UWM, and Rocket Mortgage). LendingPad exposes an Enterprise API for loan data exchange, but access is gated - it is limited to Lender Edition clients under an executed API Agreement and NDA, keys and testing-site access are issued by the support desk, and there is no public developer portal or self-serve API reference. The API entries below are honestly modeled from the vendor-integration and marketplace capabilities LendingPad describes publicly; endpoint-level surfaces are not published and are not fabricated here.

**Areas:** Mortgage · Loan Origination System · LOS · Lending · Fintech · Financial Services · Real Estate · Partner API · Gated API

## LendingPad on APIs.io

Everything profiled for LendingPad is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/lendingpad/](https://apis.io/providers/lendingpad/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [LendingPad Loans API (modeled)](https://apis.io/apis/lendingpad/lendingpad-loans-api/) — Modeled loan-file exchange surface - create, read, and update mortgage loan files, submit loan data to lenders/investors, and import/export loan data…
- [LendingPad Documents & Conditions API (modeled)](https://apis.io/apis/lendingpad/lendingpad-documents-conditions-api/) — Modeled document and condition exchange surface - push borrower and loan documents into the LendingPad LOS (as POS/doc-prep partners like Floify and…
- [LendingPad Pricing & Product Eligibility API (modeled)](https://apis.io/apis/lendingpad/lendingpad-pricing-eligibility-api/) — Modeled product, pricing, and eligibility (PPE) exchange surface - integrations with pricing engines such as Polly, Lender Price, Optimal Blue, and LoanNex…
- [LendingPad Webhooks & Events (modeled)](https://apis.io/apis/lendingpad/lendingpad-webhooks-events-api/) — Modeled event/notification surface - partner integrations describe synchronization of field updates, critical dates, and loan-status changes back to…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Lendingpad Domain Security](https://apis.io/security/lendingpad/lendingpad-domain-security/)
- [Lendingpad Trust Center](https://apis.io/security/lendingpad/lendingpad-trust-center/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Lendingpad Plans Pricing](https://apis.io/plans/lendingpad/lendingpad-plans-pricing/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://lendingpad.com)
- [Documentation](https://lendingpad.com/api-terms)
- [Blog](https://blog.lendingpad.com)

## API Evangelist rating

**Kin Score 11.1** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 0.0 |
| Contract governance | 0.0 |
| Operational transparency | 0.0 |
| Developer ergonomics | 11.9 |
| Access clarity | 15.8 |

**Agent readiness 0.0** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 10.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/lendingpad/](https://apis.io/providers/lendingpad/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for LendingPad: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/lendingpad/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
