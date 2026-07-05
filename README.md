# LendingPad (lendingpad)

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
