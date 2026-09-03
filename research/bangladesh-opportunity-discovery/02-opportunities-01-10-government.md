# Opportunities 1–10 — Government & Public Administration

> Sizing convention: **BDT 122 = USD 1** [ASSUMPTION]. TAM = total value of the activity addressed. SAM = the share realistically addressable by one well-run operator/consortium within a decade. SOM = plausible 3–5 year capture. All sizing is **[CALCULATED]** from **[VERIFIED]** inputs unless marked otherwise.

---

## Opportunity #1 — Bangladesh Data Exchange (BDX): a national interoperability layer

### 1. The Core Idea
A government-mandated, federated data-exchange layer that lets any authorised public or private system query any other system's authoritative data — with the citizen's consent, a full audit log, and no central data lake. Agencies keep their own databases; BDX standardises the pipes, the security model, and the consent record. It is the plumbing that makes "once-only" government possible: a citizen never submits a document the state already holds.

### 2. Bangladesh Problem
Gaps 1, 11, 12, 15, 16, 77, 80, 111. NID, land, tax, e-GP, health, social protection and MFS systems are silos. Every service duplicates identity verification and document collection. Social protection cannot deduplicate beneficiaries; health has no continuity of record; SME lending cannot see tax or utility data.

### 3. International Benchmark
- **Estonia — X-Road**, operated by the Information System Authority (RIA), production since **2001**. Now the backbone connecting **99% of government services**.
- **India — India Stack / Account Aggregator**, National Payments Corporation of India and Sahamati, from **2016**.
- **Rwanda — IremboGov** (RwandaOnline Platform Ltd + Government of Rwanda, **2015**) as the citizen-facing layer over the same idea.

### 4. Proof That It Works
- Estonia's X-Road handles ~**295 million requests per month**; only ~3% are triggered by direct citizen interaction — the rest is machine-to-machine. Estonia estimates **>820 years of working time saved annually**, and attributes roughly **2% of GDP** in savings to digital signatures alone. [VERIFIED]
- IremboGov: **>25 million applications**, ~**USD 300 million** in transactions, **>100 million working hours saved**, 300,000–500,000 applications/month, 80% completed online, **funded by commission on paid applications** — a self-sustaining PPP, not a grant project. [VERIFIED]

### 5. Bangladesh Current Situation
**Absent (A) as a national layer; Fragmented (C) in effect.** Bangladesh has strong *components* — NID, e-GP since 2011, MFS with 239.3m accounts, Binimoy/Bangla QR interoperability launched fully 1 Nov 2025 — but no general-purpose, legally mandated inter-agency data exchange with a consent ledger. [VERIFIED on components; ASSUMPTION that no equivalent layer exists — this must be re-verified with the ICT Division and Bangladesh Computer Council before any investment decision.]

### 6. The Bangladesh Opportunity
Bangladesh has the two things that usually block this: **a working national ID** and **a population already transacting digitally at scale**. What is missing is the middleware. And unlike Estonia in 2001, Bangladesh can copy a mature open-source implementation (X-Road is open source and used by Finland, Iceland, Ukraine, Japan and others) rather than invent one. This is the single highest-leverage item in this dossier because at least twelve other opportunities here (2, 4, 6, 8, 10, 35, 40, 42, 44, 46, 47) get materially cheaper once it exists.

### 7. Localization
- **Do not build a central data lake.** Bangladesh's political economy makes centralised data custody contested and a security liability. Federated query with audit logs is both cheaper and more politically survivable.
- **Consent must work for low-literacy users**: OTP-plus-voice confirmation in Bangla, and an agent-assisted consent flow through the existing union digital centre and MFS agent networks, not an app-only flow.
- **Start with three high-pain, low-controversy corridors** — NID↔land, NID↔education certificates, NID↔trade licence — rather than health or law enforcement, which will stall the programme politically.
- **Charge per transaction**, Irembo-style, so the operator is incentivised toward uptime and adoption instead of milestone billing.

### 8. Who Could Implement It?
**PPP** between the ICT Division / Bangladesh Computer Council (mandate, standards) and a private operator consortium (build, run, support). A local systems integrator + an X-Road implementation partner (Nortal, Cybernetica, or an Indian/Estonian SI) + a domestic telco or data-centre operator.

### 9. Business / Funding Model
**B2G + transaction fee.** Government pays an availability fee for the core; the operator earns a per-successful-transaction commission on paid citizen services and a per-query fee from regulated private consumers (banks, insurers, NBFIs) who query authoritative data with consent. Irembo demonstrates this is sufficient for sustainability.

### 10. Target Users / Beneficiaries
- **Pays:** government (availability fee), banks/insurers/telcos (query fees), citizens indirectly via service fees.
- **Uses:** civil servants, bank onboarding teams, insurers, hospitals.
- **Benefits:** citizens (documents no longer re-collected), Treasury (deduplicated benefits), lenders (verifiable data).

### 11. Estimated Market Potential
- **TAM [CALCULATED]:** Bangladesh's administrative burden is not directly measured. Using Estonia's transaction intensity scaled by population and discounting heavily for digital maturity: at 175m people and a conservative 2 verified inter-agency queries per citizen per year at Tk 15/query → **~Tk 5.3bn/yr (~USD 43m/yr)** in pure exchange fees, plus the paid-service commission pool.
- **SAM [CALCULATED]:** the paid government-service transaction pool. Rwanda processed ~USD 300m of transactions cumulatively for ~14m people. Bangladesh has 12.5× the population and higher fee levels; a mature platform plausibly intermediates **Tk 150–400bn/yr (USD 1.2–3.3bn)** in government fees, on which a 1–2% commission is **Tk 1.5–8bn/yr**.
- **SOM (5 yr) [ASSUMPTION]:** Tk 2–4bn/yr revenue for the operator.
- **The real prize is not the fee** — it is the ~2% of GDP efficiency effect Estonia claims, which on a USD 500bn economy is **USD ~10bn/yr** of avoided friction. [CALCULATED from a VERIFIED Estonian claim; heavily discount for context.]

### 12. Economic / Social Impact
Government efficiency is the primary channel. Secondary: unlocks cash-flow SME lending (Opp 44), insurance underwriting (46), targeted social protection, and a credible property market (2). Employment effect is modest directly (hundreds), enormous indirectly.

### 13. Technology Required
Open-source data-exchange middleware (X-Road or equivalent), PKI and digital signature, consent ledger, API gateway, national ID integration, cloud/colocation, security operations centre. **No blockchain required** — a signed, append-only audit log is sufficient and cheaper.

### 14. Government Role
- **Ministry/agency:** ICT Division; Bangladesh Computer Council; a2i/Aspire successor programme; Bangladesh Bank for financial-sector queries.
- **Government does:** legislate a once-only principle and a data-exchange mandate; designate authoritative data custodians; fund the core.
- **Private does:** build, operate, integrate, support, and sell to regulated private consumers.
- **PPP:** appropriate — Irembo is the template.
- **Policy change required:** a Data Exchange & Once-Only Act, or an equivalent instrument under existing ICT law, plus a consent framework.

### 15. Major Barriers
Institutional resistance (data ownership is power); procurement (a multi-year availability contract is unusual for Bangladeshi procurement); security incident risk — note Binimoy's early security failures as a live warning; political change altering the sponsor.

### 16. Difficulty of Implementation
**8/10.** Technically well-trodden; politically hard.

### 17. Opportunity Potential
**10/10.** Foundational, defensible, and it multiplies a dozen other opportunities.

### 18. Why Now?
Three conditions converged: full payment interoperability launched November 2025; NID coverage is deep; and post-2024 reform politics has created an unusual window for institutional redesign. Also, X-Road is now mature open source — the build cost in 2026 is a fraction of what Estonia spent.

### 19. First 12-Month Pilot
- **Location:** Dhaka + one district (Feni is a sensible choice — a large-scale land-record digitisation pilot has already run there with UNDP).
- **Users:** 3 agencies, 2 banks, ~50,000 citizen transactions.
- **Partners:** ICT Division, Bangladesh Bank, one private bank, one SI.
- **Budget [ASSUMPTION]:** Tk 25–45 crore (USD 2–3.7m) for core + 3 integrations.
- **Timeline:** 3 months legal/standards, 6 months build, 3 months live pilot.
- **KPIs:** documents eliminated per transaction; median service time before/after; query volume; uptime ≥99.5%.
- **Success:** ≥40% reduction in documents demanded on the three pilot services and a signed mandate to extend to 10 agencies.

### 20. OceanBlu / Entrepreneur Opportunity
A startup cannot own the mandate — but it can own the **integration layer and the private-sector consumer side**. Build first: a *consent-based data-verification API* for banks and insurers, initially wrapping whatever authoritative sources are already accessible, so it has a business with or without the government mandate. Partner: one large private bank as design partner and first customer. Moat: integrations are slow and sticky; the first mover accumulates connectors that competitors must rebuild one by one. Scale: from finance into insurance, telco, health, and then become the natural operator when the national mandate arrives.

---

## Opportunity #2 — Conclusive land titling with a title-guarantee fund

### 1. The Core Idea
Move Bangladesh from *presumptive* land records (a khatian records possession, not title) to *conclusive* title backed by a state-backed indemnity fund — combined with drone/GNSS re-survey, reconciliation of the three record-holding offices, and a digital mutation-and-registration workflow where registration automatically updates the record of rights.

### 2. Bangladesh Problem
Gap 2. Around **80% of rural court cases are land disputes** and **more than 4 million land cases are pending**. Land is the primary store of household wealth and the primary collateral class — and it cannot be reliably pledged, sold, or inherited without litigation risk. [VERIFIED]

### 3. International Benchmark
- **Rwanda — Land Tenure Regularisation** (Rwanda Natural Resources Authority, 2009–2013): systematic, low-cost, adjudication-based titling of the whole country.
- **India — SVAMITRA/SVAMITVA** (Ministry of Panchayati Raj, 2020): drone survey of inhabited rural land to issue property cards.
- **Estonia / Georgia**: registry-and-guarantee model where the register itself is the legal title.
- **Feni, Bangladesh — UNDP-supported large-scale land record digitisation pilot** (recent) — a domestic precedent to build from. [VERIFIED that this pilot exists]

### 4. Proof That It Works
Authorities themselves expect digitisation to cut land litigation **by up to 30% within five years**. [VERIFIED — note this is an official expectation, not a measured outcome; treat as a target.] Rwanda's programme is the most-cited low-cost systematic titling exercise globally and is documented in World Bank land governance literature. India's drone-based property-card issuance demonstrates the unit-cost achievable at scale in a South Asian administrative context.

### 5. Bangladesh Current Situation
**Underperforming (D).** Digitisation began via PPP as far back as **January 2010**; land records are partially digitised; e-mutation and e-porcha exist; a large-scale Feni pilot is running. But the legal character of the record is unchanged — it is still evidence of possession, not guaranteed title — and the three offices remain unreconciled. So the digitisation has automated an unreliable record rather than made it reliable. [VERIFIED on the 2010 PPP start and the Feni pilot; ASSUMPTION on the reconciliation status, to be confirmed with the Ministry of Land.]

### 6. The Bangladesh Opportunity
Bangladesh has the world's highest land value per capita relative to income in one of the most densely populated countries. The value unlocked by making title bankable is larger here than almost anywhere. And the enabling work — survey, digitisation — is already half-paid-for. The missing piece is legal (conclusive title + indemnity) and institutional (one custodian), not technological.

### 7. Localization
- **Do not attempt national conclusive title in one step.** Declare conclusive title *district by district*, only after a publicised adjudication window and a settled dispute count below a threshold. Rwanda's sequencing lesson.
- **Fund the indemnity from transaction fees**, not the budget: a small levy on every registration builds the guarantee fund, so the system pays for its own risk.
- **Use the existing union digital centre network** as the adjudication front desk — Bangladesh's real advantage over Rwanda in 2009.
- **Female co-ownership must be defaulted in**, as Rwanda did, or titling will formalise existing exclusion.
- **Handle char land and accreted/eroded land explicitly** — a Bangladesh-specific problem with no international template; needs a dynamic-boundary rule, not a static cadastre.

### 8. Who Could Implement It?
**Government-led (Ministry of Land, Directorate of Land Records and Surveys) with PPP delivery.** Private roles: drone/GNSS survey firms, data-entry and adjudication logistics, software, and — a genuinely commercial slot — **title insurance underwriters** once the register is reliable.

### 9. Business / Funding Model
**B2G procurement for survey and systems + transaction fee + title insurance premium.** The insurance layer is where a private company can build a durable business: title insurance is a standard product in the US and increasingly in India, and it becomes viable the moment the register is good enough to underwrite against.

### 10. Target Users / Beneficiaries
- **Pays:** buyers and sellers (registration fee/levy), lenders (title insurance), government (systems).
- **Uses:** citizens, banks, developers, courts.
- **Benefits:** ~everyone with land; the banking system (a new collateral class); the courts (docket relief).

### 11. Estimated Market Potential
- **TAM [ASSUMPTION]:** the value of annual land transactions in Bangladesh is not published reliably; do not invent a number. What *is* defensible: >4m pending land cases each carrying legal costs, and a national land stock that is the dominant household asset class.
- **SAM [CALCULATED]:** survey + digitisation + systems for a national programme, benchmarked on India's drone-survey unit costs, plausibly **Tk 30–80bn (USD 250–650m)** of multi-year public procurement.
- **SOM [CALCULATED]:** title insurance. If even 200,000 transactions a year are insured at an average premium of Tk 15,000 → **Tk 3bn/yr (USD 24.6m/yr)** in premium, growing with formalisation.

### 12. Economic / Social Impact
Court docket relief (the single largest category of pending litigation); collateral creation for SME and agricultural lending; reduced land-related violence; higher municipal own-source revenue once a property register exists (links to Opp 5). Poverty impact is concentrated among women and heirs, who lose most from unenforceable claims.

### 13. Technology Required
Drone/UAV photogrammetry, GNSS/CORS network, GIS cadastre, workflow software linking sub-registrar ↔ AC Land ↔ survey, digital signature, and integration to the BDX layer (Opp 1). Blockchain is **not** required and adds cost without solving the adjudication problem, which is social not cryptographic.

### 14. Government Role
- **Ministry of Land**; Directorate of Land Records and Surveys; Law and Justice Division for the conclusive-title statute; Ministry of Finance for the indemnity fund.
- **Government:** legislate; adjudicate; guarantee. **Private:** survey; software; insure.
- **Policy change:** amendment to make the register conclusive with statutory indemnity — the single most consequential legal reform in this dossier.

### 15. Major Barriers
Political economy of land (the most contested asset in Bangladesh); institutional resistance from three separate offices; capital; capacity for adjudication at scale; risk that digitisation entrenches fraudulent records if adjudication is skipped.

### 16. Difficulty of Implementation
**9/10.**

### 17. Opportunity Potential
**10/10.**

### 18. Why Now?
The Feni pilot creates a live template. Court backlog has become a headline political problem (4.64m cases). And LDC graduation raises the premium on domestic investment and collateral formation.

### 19. First 12-Month Pilot
- **Location:** one upazila in Feni (building on the existing pilot) plus one peri-urban upazila near Gazipur where land values are high and disputes are frequent.
- **Users:** ~80,000–150,000 parcels.
- **Partners:** Ministry of Land, DLRS, UNDP, a survey contractor, one bank willing to pilot title-backed lending.
- **Budget [ASSUMPTION]:** Tk 20–40 crore.
- **KPIs:** parcels adjudicated; disputes raised and resolved in the objection window; % of parcels with female co-ownership recorded; time-to-mutation; number of bank loans secured on pilot titles.
- **Success:** time-to-mutation below 30 days, <2% unresolved objections, and at least one bank lending against pilot titles.

### 20. OceanBlu / Entrepreneur Opportunity
Realistic entry is **not** the register — it is the services around it. Build first: a **land due-diligence and title-search service** (people already pay lawyers and touts for this, opaquely) productised as a paid report combining porcha, mutation, mouza map and encumbrance checks. That is a business today, with no legal reform required, and it generates the proprietary dataset that makes you the natural title insurer later. First customers: real-estate developers and banks' credit departments. Moat: the accumulated search dataset and the relationships with sub-registrar offices. Scale: report → insurance → registry services.

---

## Opportunity #3 — Online Dispute Resolution and a digital small-claims track

### 1. The Core Idea
A statutory online dispute resolution (ODR) channel for low-value civil, consumer, tenancy, cheque-dishonour and small commercial disputes: file online, structured negotiation, then online mediation, then a documents-only adjudication with a binding, enforceable outcome — diverting a large volume of cases from a court system that cannot absorb them.

### 2. Bangladesh Problem
Gap 3. **4,639,476 cases pending** as of 31 March 2026; High Court judges carry an average of **~6,463 cases each** and clear ~435/year. At that ratio the backlog is not clearable by adding judges alone. [VERIFIED]

### 3. International Benchmark
- **China — Internet Courts** (Hangzhou 2017, Beijing and Guangzhou 2018), Supreme People's Court: fully online litigation for defined case categories.
- **United Kingdom — Online Civil Money Claims / HMCTS reform** (from 2018).
- **India — SAMA, Presolv360, and the NITI Aayog ODR policy push** (2020–): private ODR platforms integrated with lenders and regulators — the most transferable model for Bangladesh because it is *private-sector-led with regulatory blessing*.
- **Brazil — consumidor.gov.br** (federal consumer platform, 2014).

### 4. Proof That It Works
consumidor.gov.br is the cleanest evidence class: a government-run online consumer dispute platform with published resolution rates and response times, operating for over a decade at national scale [VERIFIED that the platform exists and is long-running; specific rates should be re-pulled from the platform's own published indicators before use in an investment memo]. China's internet courts demonstrate that documents-only online adjudication can be run at very high volume. India's ODR ecosystem demonstrates the *private* version can be commercially viable through lender-paid fees.

### 5. Bangladesh Current Situation
**Absent (A) for ODR; Early-stage (B) for court digitisation.** Bangladesh has run virtual courts and has established a Supreme Court Secretariat as part of 2025 reforms, but **no progress has been made in reducing the case backlog**, and there is no ODR track. [VERIFIED]

### 6. The Bangladesh Opportunity
Bangladesh has the two ingredients India used: a huge volume of small-value financial disputes (MFS, microfinance, consumer credit, cheque cases) and near-universal mobile reach. Crucially, most of these disputes are between a *repeat institutional player* (a bank, an MFI, an MFS provider, a retailer) and an individual — and repeat players will pay for fast resolution, which is what makes the model self-financing.

### 7. Localization
- **Start outside the courts, not inside them.** Begin as contractual pre-litigation ODR embedded in MFI, MFS and consumer-credit contracts. This needs no legislation — only enforceable arbitration/mediation clauses under existing law.
- **Bangla-first, voice-first, phone-number-identity.** Most claimants will not use a web portal; design for IVR, WhatsApp/IMO and agent-assisted filing at union digital centres.
- **Mediators drawn from retired judges, lawyers and trained non-lawyers** — Bangladesh has a lawyer surplus and a judge deficit; use the surplus.
- **Village court (gram adalat) integration** is the distinctive Bangladeshi asset: a statutory local dispute forum already exists and is chronically under-used. Digitising and supporting gram adalat is likely a faster path than a new institution.

### 8. Who Could Implement It?
**Startup or social enterprise, with government and Bangladesh Bank as enablers.** Later: PPP with the Law and Justice Division and the Supreme Court for a formal small-claims track.

### 9. Business / Funding Model
**B2B per-case fee paid by institutional users** (banks, MFIs, MFS providers, e-commerce platforms, insurers) — the India ODR model. Later, **B2G** for a court-annexed track. Cross-subsidy: institutional fees fund free access for individual claimants.

### 10. Target Users / Beneficiaries
- **Pays:** lenders, MFS providers, retailers, insurers.
- **Uses:** their customers and their recovery teams.
- **Benefits:** claimants (resolution in weeks, not years), courts (docket relief), the credit system (faster recovery lowers the risk premium in interest rates).

### 11. Estimated Market Potential
- **TAM [CALCULATED]:** if even 15% of the 4.64m pending cases are low-value civil/consumer matters, that is ~700,000 legacy disputes, plus new flow. At a modest Tk 2,500 per resolved case → **~Tk 1.75bn** on the backlog alone, recurring on new flow.
- **SAM [CALCULATED]:** Bangladesh's MFI sector alone serves tens of millions of borrowers; the annual dispute/default flow across MFI + MFS + consumer credit plausibly generates **1–3m disputes/yr**. At Tk 800–2,500 per case → **Tk 0.8–7.5bn/yr (USD 6.5–61m/yr)**.
- **SOM (3–5 yr) [ASSUMPTION]:** Tk 200–600m/yr.

### 12. Economic / Social Impact
Direct: faster resolution reduces the cost of credit and improves contract enforcement — a first-order determinant of investment. Employment: several thousand trained mediators, a new professional category, well-suited to women and to law graduates who cannot get court practice. Government efficiency: measurable docket relief.

### 13. Technology Required
Case-management workflow, secure video, e-signature, Bangla NLP for triage and summarisation, mobile/IVR channels, payment integration. Modest, well-understood stack. AI is genuinely useful here for triage and drafting — but the adjudication must remain human, or the outcomes will not be trusted or enforceable.

### 14. Government Role
- **Law and Justice Division**; Supreme Court; Bangladesh Bank (to permit/encourage ODR clauses in regulated lending); Ministry of Local Government for gram adalat.
- **Government:** recognise ODR outcomes as enforceable; ideally a small-claims statute with an online default track.
- **Private:** run the platform, train and manage mediators, sell to institutions.
- **PPP:** appropriate at the court-annexed stage; unnecessary at the start.

### 15. Major Barriers
Enforceability of outcomes without legislation; bar association resistance (a real and well-organised interest); public trust in a non-court forum; data protection.

### 16. Difficulty of Implementation
**6/10** as a private pre-litigation service; **9/10** as a court-annexed statutory track.

### 17. Opportunity Potential
**8/10.**

### 18. Why Now?
The backlog has grown to a politically salient 4.64m; judiciary reform is explicitly on the 2025–26 agenda with the Supreme Court Secretariat established; and full payments interoperability (Nov 2025) is about to increase the volume of small digital financial disputes sharply.

### 19. First 12-Month Pilot
- **Location:** Dhaka + Chattogram, remote-first.
- **Users:** 3 institutional clients (1 bank, 1 large MFI, 1 MFS provider), 10,000–25,000 disputes.
- **Partners:** an MFI network, Bangladesh Bank (no-objection), a law school for mediator training.
- **Budget [ASSUMPTION]:** Tk 6–12 crore.
- **KPIs:** median days to resolution; settlement rate; cost per case; recovery rate vs the institution's litigation baseline; claimant satisfaction.
- **Success:** median resolution <30 days, settlement rate >55%, and cost per case below one-third of the institution's litigation cost.

### 20. OceanBlu / Entrepreneur Opportunity
Yes — this is one of the most realistic startup entries in the dossier because **it needs no law change to begin**. Build first: a mediation-and-settlement workflow for one MFI's overdue-loan portfolio, priced per resolved case. First customer: a large MFI or an MFS lender, both of whom currently write off recoverable balances because litigation is uneconomic. Moat: outcome data (which disputes settle, at what discount, with which script) becomes a pricing asset no competitor has; plus institutional integrations. Scale: MFI → banks → e-commerce and insurance → court-annexed contract.

---

## Opportunity #4 — Mandatory VAT e-invoicing with a revenue-analytics layer

### 1. The Core Idea
A national electronic invoicing regime where every B2B and larger B2C invoice is validated in real time against a government platform before it is legally valid, creating a continuous transaction data stream. Layered on top: analytics that detect VAT fraud rings, missing-trader chains and under-declaration, and — critically — a data-sharing facility that lets compliant firms use their own verified invoice history to borrow.

### 2. Bangladesh Problem
Gap 4. Tax/GDP fell to **6.56% in FY25** from 7.2% in FY24 — among the lowest in the world — and NBR missed its FY25 target by **Tk 92,625 crore**, collecting Tk 3,70,874 crore, ~3.08% *below* the prior year. The NBR itself targets only 10.5% by FY35. Without revenue, none of the public investment implied by the rest of this dossier is financeable. [VERIFIED]

### 3. International Benchmark
- **Brazil — Nota Fiscal Eletrônica (NF-e)**, state revenue secretariats + SEFAZ, national from **2008**: the world's largest mandatory e-invoicing system.
- **India — GST e-invoicing / e-way bill** (GSTN, e-invoicing from **2020**, progressively lowered turnover thresholds).
- **Türkiye — e-Fatura** (Revenue Administration, **2012**).
- **Chile, Mexico, Italy** — long-running mandatory regimes.

### 4. Proof That It Works
Latin American e-invoicing is the most-studied revenue-administration reform of the last twenty years, with IMF and IDB literature documenting VAT compliance gains; India's e-invoicing plus e-way bill regime is credited with sharply improving GST compliance and is now extended to progressively smaller firms — the extension itself is the revealed-preference evidence that it works. [VERIFIED that these regimes exist, are long-running, and have been progressively expanded — the strongest available signal. Specific percentage revenue gains should be sourced from IMF/IDB country papers before being quoted in a board memo; do not use vendor-published figures.]

### 5. Bangladesh Current Situation
**Underperforming (D).** Bangladesh has deployed Electronic Fiscal Devices/EFD machines for retail VAT and has a VAT online system, but coverage is partial, EFD rollout has been slow, and there is no comprehensive real-time invoice-clearance regime for B2B. The result: the VAT chain has holes at exactly the points where fraud occurs. [ASSUMPTION on current EFD coverage — must be verified with NBR before investment; the tax/GDP outcome is VERIFIED and is itself strong evidence the current approach is not working.]

### 6. The Bangladesh Opportunity
Two things make Bangladesh unusually suited. First, the corporate sector is **concentrated**: RMG, pharma, telecom, banking and FMCG account for a large share of formal B2B value, so a threshold-based rollout captures most of the base quickly with few taxpayers. Second, e-invoicing creates the **single most valuable dataset in the country for SME lending** (Opp 44) — which gives firms a reason to *want* to be inside the system, turning a compliance burden into a credit benefit. That framing is what made India's system politically survivable.

### 7. Localization
- **Sequence by turnover, starting high.** Top 5,000 firms first; do not start with small retail, which is where EFD rollout has repeatedly stalled.
- **Free government-provided invoicing app for small firms**, plus certified private providers for large ones — the Brazilian/Indian hybrid.
- **Bundle the carrot with the stick from day one:** a compliant firm's verified invoice history should be shareable, with consent, to lenders through the BDX layer (Opp 1). Bangladesh should not repeat the mistake of selling e-invoicing purely as enforcement.
- **Design for intermittent connectivity**: offline invoice generation with deferred clearance and a signed local hash, as India's e-way bill does.

### 8. Who Could Implement It?
**Government (NBR) with private certified service providers.** The commercial opportunity for entrepreneurs is the **provider layer** — invoicing software, ERP connectors, reconciliation tools, and analytics — exactly as GSPs/ASPs became an industry in India.

### 9. Business / Funding Model
For government: revenue self-funding, by a very large margin. For private providers: **SaaS subscription + per-invoice fee + ERP integration services**, and later data-derived products (financing, reconciliation, working-capital tools).

### 10. Target Users / Beneficiaries
- **Pays:** businesses (software fees); government (platform).
- **Uses:** every VAT-registered firm and their accountants.
- **Benefits:** Treasury; compliant firms (levelled playing field and credit access); lenders.

### 11. Estimated Market Potential
- **TAM [CALCULATED]:** the fiscal prize dominates. Moving tax/GDP from 6.56% to the NBR's own 10.5% target on a ~USD 500bn economy is **~USD 20bn/yr** of additional revenue. Even one percentage point is ~USD 5bn/yr. This is the largest single number in this dossier.
- **SAM (private provider market) [CALCULATED]:** if 150,000–300,000 firms eventually transact electronically at Tk 8,000–20,000/yr for software and services → **Tk 1.2–6bn/yr (USD 10–49m/yr)**.
- **SOM [ASSUMPTION]:** Tk 300–800m/yr for a leading provider within 5 years.

### 12. Economic / Social Impact
Government efficiency and fiscal space are the primary channels — and fiscal space is the binding constraint on health, education and infrastructure spending. Secondary: formalisation, SME credit access, and a level playing field that stops penalising compliant firms.

### 13. Technology Required
Invoice registration portal, digital signature, QR/IRN, high-throughput API infrastructure, ERP connectors, fraud analytics (network analysis on invoice graphs is genuinely the right use of ML here), and offline-tolerant clients.

### 14. Government Role
- **NBR** (VAT Wing), Internal Resources Division, Ministry of Finance; IMF programme conditionality is a supporting lever.
- **Government:** mandate, thresholds, platform, penalties.
- **Private:** everything above the API.
- **Policy change:** amendment to VAT and Supplementary Duty rules making a cleared electronic invoice the only legally valid invoice above a threshold.

### 15. Major Barriers
Institutional resistance inside the revenue administration (discretion is valuable); business resistance and lobbying; connectivity; the political sensitivity of any visible tax tightening; the risk of a botched rollout discrediting the concept — Bangladesh's EFD experience is the cautionary precedent.

### 16. Difficulty of Implementation
**8/10.**

### 17. Opportunity Potential
**10/10** (for the country); **7/10** (for a private firm, which captures only the provider layer).

### 18. Why Now?
Revenue collection actually *fell* in FY25 while LDC graduation in November 2026 removes trade-preference-linked revenue comfort and increases the need for domestic resource mobilisation. There is an explicit reform target (10.5% by FY35) and IMF engagement. The window is now.

### 19. First 12-Month Pilot
- **Location:** national, by turnover threshold.
- **Users:** top 1,000–2,000 VAT payers.
- **Partners:** NBR, 2–3 certified software providers, ERP vendors, a business chamber (DCCI/MCCI) for change management.
- **Budget [ASSUMPTION]:** Tk 40–90 crore for the clearance platform and analytics.
- **KPIs:** % of pilot-firm invoices cleared electronically; input-tax credit mismatch rate; VAT collected from pilot cohort vs counterfactual; average clearance latency.
- **Success:** >90% of pilot invoices cleared electronically, measurable reduction in credit mismatches, and a legislated threshold-lowering schedule.

### 20. OceanBlu / Entrepreneur Opportunity
Do not try to be the government platform. Be the **provider**. Build first: an invoicing and VAT-reconciliation SaaS for mid-sized firms that works *today* against existing VAT rules, so it has customers before any mandate — then become certified on day one when the mandate lands. First customers: RMG suppliers and pharma distributors with complex input-credit chains. Moat: ERP integrations and reconciliation accuracy; switching cost is very high once a firm's ledger runs through you. Scale: invoicing → reconciliation → invoice-backed working capital (Opp 44), which is where the real margin is.

---

## Opportunity #5 — National digital address and property register

### 1. The Core Idea
A single authoritative register of every structure and plot in Bangladesh with a permanent machine-readable address code and geolocation — issued once, used by everyone: post, e-commerce, utilities, ambulances, census, tax, and municipal billing. It is the physical-world equivalent of the NID.

### 2. Bangladesh Problem
Gap 5, and it silently causes gaps 13 and 31. Bangladeshi addresses are descriptive, not systematic ("beside the mosque, third lane"). Every e-commerce delivery, every utility connection, every ambulance dispatch, and every municipal tax assessment re-solves the same problem privately and expensively. Local governments have almost no own-source revenue partly because there is no property register to tax against.

### 3. International Benchmark
- **Ghana — GhanaPostGPS** (Ghana Post + Vokacom, **2017**): national digital addressing covering the whole country.
- **India — SVAMITVA property cards** (2020) and the postal PIN + DIGIPIN initiative.
- **Rwanda — national addressing system** as part of its digital government programme.
- **South Africa, Colombia, Ireland (Eircode, 2015)** — national address code systems in mixed-formality contexts.

### 4. Proof That It Works
Ireland's Eircode is the cleanest developed-market proof that a unique-per-property code can be retrofitted onto an unstructured address system nationally and monetised through licensed data access [VERIFIED that Eircode exists and operates on a licensing model]. Ghana demonstrates feasibility in a low-formality African context at national scale. India's SVAMITVA demonstrates drone-based property mapping at very large scale in a South Asian administrative setting. [VERIFIED existence and scale; quantitative impact evaluations are thinner for this category than for most others in this dossier — that is an honest weakness of the evidence base here.]

### 5. Bangladesh Current Situation
**Absent (A).** Bangladesh has postcodes at a coarse level and multiple private geocoding efforts by logistics and ride-hailing companies, each proprietary and partial. There is no national property/address authority. [ASSUMPTION — to be verified with the Ministry of Posts and Telecommunications and Bangladesh Post before investment.]

### 6. The Bangladesh Opportunity
Bangladesh has among the world's highest population densities, one of Asia's fastest-growing e-commerce and quick-commerce sectors, and a near-total absence of address infrastructure. The cost of the gap is being paid every day by delivery riders making phone calls. Meanwhile the *fiscal* upside — a property register enabling municipal own-source revenue — is arguably larger than the logistics upside and is entirely unexploited.

### 7. Localization
- **Address the structure, not the parcel, first.** Parcels are legally contested (Opp 2); buildings are not. Mapping structures avoids the land-dispute quagmire and still delivers the logistics and municipal-revenue benefits.
- **Crowdsource the last mile through the people already doing it**: pay delivery riders and MFS agents per verified structure captured. This is how you map 40 million structures affordably.
- **Bangla-friendly code format** — memorable, speakable over a phone, and short enough to write on a parcel.
- **Free for citizens and emergency services; licensed to commercial users.** Eircode's model.
- **Anticipate erosion and flooding**: char and riverbank structures change; the register needs a lifecycle state, not just a creation event.

### 8. Who Could Implement It?
**PPP** — Bangladesh Post or the ICT Division as custodian; a private operator for capture, maintenance and commercial licensing. Strong fit for a consortium including a logistics company, a telco and a mapping firm.

### 9. Business / Funding Model
**Data licensing + B2G.** Free public lookup; paid API for e-commerce, logistics, utilities, banks (KYC address verification), and insurers. Municipal governments pay for the property-assessment dataset — and it pays for itself out of the property tax it enables.

### 10. Target Users / Beneficiaries
- **Pays:** logistics/e-commerce firms, utilities, banks, municipalities.
- **Uses:** delivery riders, meter readers, ambulance dispatch, census enumerators, tax assessors.
- **Benefits:** citizens (they can be found), municipalities (revenue), emergency services (response time).

### 11. Estimated Market Potential
- **TAM [CALCULATED]:** Bangladesh has roughly 40+ million households [CALCULATED from ~175m population at ~4.2 persons/household]. Municipal property tax on even a modest fraction of urban structures is the dominant value pool — potentially **tens of billions of taka annually** in currently uncollected local revenue [ASSUMPTION — no reliable published base to anchor this; flagged as the key uncertainty].
- **SAM (commercial data licensing) [CALCULATED]:** if 50m e-commerce/logistics deliveries per year are address-verified at Tk 0.50–1.00 per lookup → **Tk 25–50m/yr**, rising steeply with e-commerce growth; plus enterprise licences at Tk 20–60 lakh/yr for large users.
- **SOM [ASSUMPTION]:** Tk 100–300m/yr within 5 years for the operator; the municipal-revenue effect is public, not private.

### 12. Economic / Social Impact
Logistics productivity (failed-delivery rates in Bangladesh are high and entirely address-driven); emergency response times; municipal fiscal capacity — which is the precondition for cities managing their own waste, water and roads (Opps 13–15). Employment: several thousand field enumerators during capture.

### 13. Technology Required
GNSS capture app, satellite/drone imagery, geocoding engine, address-matching/fuzzy-search in Bangla, API infrastructure, integration with BDX (Opp 1).

### 14. Government Role
- **Ministry of Posts and Telecommunications / Bangladesh Post**; ICT Division; Local Government Division; Bangladesh Bureau of Statistics.
- **Government:** designate the register as authoritative and require its use in government services and utility connections — without a use mandate, adoption fails, which is the main lesson from address projects that stalled elsewhere.
- **Private:** capture, maintain, license.
- **PPP:** yes.

### 15. Major Barriers
Adoption without a mandate; maintenance funding (registers rot without recurring revenue); custodianship disputes between agencies; privacy concerns around a structure-level register.

### 16. Difficulty of Implementation
**6/10.**

### 17. Opportunity Potential
**7/10** commercially; **9/10** as enabling infrastructure.

### 18. Why Now?
E-commerce and quick-commerce volumes have reached the point where private firms are individually spending real money solving addressing; a shared utility is now cheaper for all of them. Drone and satellite imagery costs have collapsed.

### 19. First 12-Month Pilot
- **Location:** one city corporation zone (e.g. Dhaka North Ward cluster) + one pourashava.
- **Users:** ~200,000–400,000 structures.
- **Partners:** city corporation, 2 logistics firms, 1 utility, Bangladesh Post.
- **Budget [ASSUMPTION]:** Tk 8–18 crore.
- **KPIs:** structures captured/verified; failed-delivery rate before/after for partner logistics firms; municipal assessment coverage increase; API calls.
- **Success:** ≥90% structure coverage in the pilot zone, a measurable drop in partner failed-delivery rates, and one municipality adopting it for assessment.

### 20. OceanBlu / Entrepreneur Opportunity
Strong startup fit. Build first: an **address-resolution API for e-commerce and logistics** — solve the failed-delivery problem commercially before seeking any government mandate. First customers: the large e-commerce and quick-commerce players, and the courier networks, all of whom can quantify the cost of failed deliveries. Moat: the verified-structure dataset compounds; every delivery improves it, which is a genuine data network effect — rare in Bangladesh. Scale: logistics → utilities → banks (address KYC) → municipal assessment → national custodian.

---

## Opportunity #6 — Open contracting analytics on top of e-GP

### 1. The Core Idea
Bangladesh already runs e-GP. The missing layer is **analysis**: publish procurement data in the Open Contracting Data Standard and build a red-flag engine that scores every tender for single-bidding, bid-rotation, unusual price patterns, short advertisement windows and repeat-winner concentration — with a civic monitoring interface and an internal audit workflow.

### 2. Bangladesh Problem
Gap 6. e-GP digitised transactions but did not create competitive intelligence. Evidence shows e-GP adoption already **reduces the price-to-cost ratio of contracts by 10.25–11.85%**, and that universal e-procurement coverage could save up to **USD 1.76bn per year** — meaning the remaining savings are locked behind coverage and analysis, not behind the platform itself. [VERIFIED]

### 3. International Benchmark
- **Ukraine — ProZorro** (2016) and its civic monitoring layer **DOZORRO**: the reference implementation globally, and specifically designed for a low-trust environment.
- **Open Contracting Partnership / OCDS** — adopted by Ukraine, Colombia, Paraguay, Nigeria and others.
- **Colombia — SECOP II / Colombia Compra Eficiente**.

### 4. Proof That It Works
ProZorro is the most-documented procurement transparency reform of the last decade and won international recognition for measurable savings and increased supplier participation; DOZORRO demonstrated that civic monitors, given structured data, generate actionable complaints at scale. [VERIFIED that ProZorro/DOZORRO exist, operate nationally since 2016, and are widely documented; specific savings percentages should be taken from Open Contracting Partnership evaluations rather than press before quoting.] The Bangladesh-specific e-GP evidence (10.25–11.85% price-to-cost reduction) is itself strong, locally-generated proof that procurement digitisation delivers measurable money. [VERIFIED]

### 5. Bangladesh Current Situation
**Underperforming (D).** e-GP has run since **2 June 2011** under CPTU, now the Bangladesh Public Procurement Authority (BPPA); 86% of bidders agree it reduces time, visits and costs; Tk 9,350 crore of savings was recorded in 2018-19. But the data is not published in an open standard, there is no public red-flag analytics, and Transparency International Bangladesh has published critical assessment of the system. [VERIFIED]

### 6. The Bangladesh Opportunity
This is the rare case where the expensive part — a national transactional platform with a decade of data — **already exists and is paid for**. The incremental cost of an analytics and transparency layer is trivial relative to the recoverable savings. And unlike most anti-corruption interventions, this one has a defensible commercial model: the same engine that flags collusion for the auditor also tells *suppliers* where to bid, which is a product they will pay for.

### 7. Localization
- **Lead with efficiency, not corruption.** Frame it internally as "value for money and competition analytics" for BPPA and the line ministries; a purely anti-corruption framing gets the project killed.
- **Publish a defined subset first** (tender notices, award values, winners, number of bidders) rather than everything — this is achievable without a fight and already enables most red flags.
- **Build the supplier-facing product simultaneously**: a bid-intelligence subscription for contractors is a real business in Bangladesh today, since finding relevant tenders is currently manual.
- **Engage the Implementation Monitoring and Evaluation Division (IMED)** as the analytics consumer — it has the mandate and lacks the tooling.

### 8. Who Could Implement It?
**Startup or social enterprise + BPPA**, ideally with a civic partner (TIB, or a university) for the monitoring layer, and a development partner for initial funding of the public-good component.

### 9. Business / Funding Model
Dual: **B2B subscription** (bid intelligence, competitor analysis, pricing benchmarks sold to contractors and suppliers) funds the commercial entity; **B2G licence** to BPPA/IMED/CAG for the audit and red-flag workbench. The public transparency portal is the loss-leader that creates legitimacy and data access.

### 10. Target Users / Beneficiaries
- **Pays:** contractors and suppliers (subscriptions); government (audit tooling).
- **Uses:** procurement officers, auditors, journalists, bidders.
- **Benefits:** Treasury, honest contractors (who currently lose to cartels), citizens.

### 11. Estimated Market Potential
- **TAM [CALCULATED]:** the savings pool is the anchor — up to **USD 1.76bn/yr** at full coverage per the cited estimate. Even capturing 3% of that as fee-bearing services is USD 50m/yr, though realistically government will not pay a share of savings.
- **SAM [CALCULATED]:** bid-intelligence subscriptions. Bangladesh has tens of thousands of registered government contractors; at 5,000 subscribers × Tk 30,000–100,000/yr → **Tk 150–500m/yr (USD 1.2–4.1m/yr)**.
- **SOM [ASSUMPTION]:** Tk 40–120m/yr within 3–4 years.

### 12. Economic / Social Impact
Fiscal: direct savings on the development budget. Competition: more bidders per tender is the single best-evidenced driver of price reduction. Governance: a measurable, publishable integrity indicator. This is a high-impact, low-capital opportunity — a classic hidden gem.

### 13. Technology Required
OCDS data pipeline, ETL from e-GP, anomaly detection and network analysis (co-bidding graphs), dashboards, alerting. Modest and cheap; the hard part is data access, not technology.

### 14. Government Role
- **BPPA (ex-CPTU)**, IMED, Office of the Comptroller and Auditor General, Ministry of Planning.
- **Government:** publish data in an open standard; adopt the red-flag workbench in audit workflow.
- **Private:** build and operate; sell supplier-side products.
- **Policy change:** a procurement data disclosure rule under the Public Procurement Act/Rules.

### 15. Major Barriers
Data access is the whole game — and it is controlled by the institution most exposed by the analysis. Institutional resistance; political risk; potential legal restrictions on republishing tender data.

### 16. Difficulty of Implementation
**5/10** for the commercial product; **7/10** for the government-adopted audit layer.

### 17. Opportunity Potential
**8/10.**

### 18. Why Now?
Post-2024 governance reform politics makes procurement transparency unusually saleable; fiscal stress (FY25 revenue shortfall of Tk 92,625 crore) makes savings urgent; and e-GP now has a deep enough data history for meaningful pattern analysis.

### 19. First 12-Month Pilot
- **Location:** two line ministries (e.g. LGED and Roads & Highways — the largest civil-works spenders).
- **Users:** ministry procurement and audit staff; 200–500 contractor subscribers.
- **Partners:** BPPA, IMED, one development partner, a civic organisation.
- **Budget [ASSUMPTION]:** Tk 3–7 crore.
- **KPIs:** average bidders per tender; % single-bid tenders; flagged-tender review rate; subscriber count and retention.
- **Success:** measurable increase in average bidders per tender in the pilot ministries and a signed BPPA agreement to publish in OCDS.

### 20. OceanBlu / Entrepreneur Opportunity
Excellent entrepreneurial fit: **low capital, fast to revenue, high defensibility through data**. Build first: the contractor-facing bid intelligence subscription using publicly visible tender data — revenue in months, no government permission required. First customers: mid-sized civil-works contractors who currently miss tenders. Moat: the historical award database and pricing benchmarks; nobody else will have assembled it. Scale: supplier intelligence → cartel analytics → government audit tooling → regional export (the same product works in Nepal, Sri Lanka, and East Africa).

---

## Opportunity #7 — Government-to-Government zero-fee migration corridors with a skills passport

### 1. The Core Idea
Replace the sub-agent recruitment chain with government-to-government (G2G) corridors modelled on Korea's Employment Permit System: a single public recruitment agency runs testing, skill certification, language training and placement; destination employers pay the placement cost; and the migrant's fee is capped near zero. Wrap it in a digital "skills passport" that destination-country employers can verify.

### 2. Bangladesh Problem
Gap 7 and 58. A Bangladeshi worker spends on average **Tk 416,789** to go abroad against an average monthly income of **Tk 23,693** — over **17 months** of earnings just to repay migration cost. The Singapore route costs **Tk 574,241**, roughly Tk 300,000 above the government-fixed fee. Average recruitment costs of ~**USD 3,900** compare with a G2G-Plus design target of **USD 420**. Bangladesh is repeatedly identified as having among the world's highest migration costs. [VERIFIED]

### 3. International Benchmark
- **Republic of Korea — Employment Permit System (EPS)**, Ministry of Employment and Labor + Human Resources Development Service of Korea, launched **2004**, operating under mandatory MOUs with **15 Asian origin countries** (Bangladesh among them).
- **Philippines — POEA/DMW** regulated deployment and standard employment contracts.
- **Global Skill Partnerships** (Center for Global Development framework) — train-in-origin, place-in-destination.

### 4. Proof That It Works
Before EPS, the average recruitment cost per temporary migrant worker in Korea was **USD 3,509 (2001)**; by **2014 it had fallen to USD 941** — a ~73% reduction, achieved specifically by removing private intermediaries through G2G arrangements. The EPS design explicitly eliminates labour-market intermediaries and their rent-seeking. [VERIFIED]

### 5. Bangladesh Current Situation
**Underperforming (D).** Bangladesh *participates* in EPS-Korea and has run G2G and "G2G Plus" arrangements with Malaysia — but these cover a small fraction of the roughly one-million-per-year outflow, and the G2G Plus experience showed costs drifting far above design targets. BMET sets ceilings (Tk 20,000 for some female-worker corridors; Tk 44,000–84,000 for UAE/Oman/Singapore/Malaysia private recruitment) that are routinely exceeded by an order of magnitude in practice. So the *model* exists in Bangladesh and is proven to work — it is simply not the dominant channel. [VERIFIED]

### 6. The Bangladesh Opportunity
This is the highest-value-per-taka social intervention in the dossier. Bangladesh already sends the workers and already receives **USD 32.8bn/yr** in remittance (2025 record). Cutting migration cost from ~Tk 400,000 to ~Tk 50,000 for even 200,000 workers a year returns **Tk 70bn (~USD 574m) per year directly into the hands of the poorest migrating households** — [CALCULATED: 200,000 × Tk 350,000 saved]. No new industry needs to be created; only an intermediary chain needs to be replaced.

### 7. Localization
- **Do not attempt to abolish the recruiting-agency industry.** Korea could; Bangladesh cannot — the sector is politically entrenched. Instead, **convert agencies into licensed service providers paid by employers** on a per-placement basis with published price caps, and let the state own testing, certification and matching.
- **Make the employer pay** (the "Employer Pays Principle"). This is the single most important design choice and it is achievable in corridors where destination employers face ESG/audit pressure — Japan, Korea, and increasingly Gulf construction contractors working for international clients.
- **Skill-test in Bangladesh to destination standards**, not Bangladeshi ones — the failure mode of existing TTCs.
- **Finance the pre-departure gap** with a low-cost migration loan repayable from wages, distributed through MFS and secured by the placement contract, so the migrant does not sell land.
- **Publish a public corridor price index** — transparency is the cheapest enforcement tool available.

### 8. Who Could Implement It?
**Government-led (Ministry of Expatriates' Welfare and Overseas Employment, BMET, BOESL)** with **PPP** for training and testing delivery, plus a **social enterprise** running the ethical-recruitment layer and a **bank/MFI** running migration finance. Industry association (BAIRA) engagement is unavoidable and should be structured, not fought.

### 9. Business / Funding Model
**Employer-paid placement fee** (the core), plus **B2G training contracts**, plus **migration loan interest**, plus **fee-based skills certification**. Ethical recruitment is a viable business: destination employers in audited supply chains increasingly *require* zero-fee recruitment and will pay for verified compliance.

### 10. Target Users / Beneficiaries
- **Pays:** destination employers; government (training infrastructure).
- **Uses:** migrant workers, employers, recruiters.
- **Benefits:** migrant households (the largest single beneficiary group in this dossier), the balance of payments, and destination employers who get verified skills.

### 11. Estimated Market Potential
- **TAM [CALCULATED]:** at roughly 1m departures/yr × average cost Tk 416,789, the current annual migration-cost pool paid by workers is on the order of **Tk 400bn (~USD 3.3bn) per year**. That entire pool is the addressable inefficiency.
- **SAM [CALCULATED]:** capture 20% of departures into employer-paid corridors → 200,000 placements/yr; at an employer-paid fee of Tk 60,000–120,000 → **Tk 12–24bn/yr (USD 98–197m/yr)** in legitimate, invoiced revenue replacing informal rents.
- **SOM [ASSUMPTION]:** 20,000–40,000 placements/yr within 5 years for a leading ethical operator → Tk 1.2–4.8bn/yr.

### 12. Economic / Social Impact
- **Poverty reduction:** direct and large — [CALCULATED] Tk 350,000 saved per worker is roughly 15 months of their overseas earnings retained by the household.
- **Foreign exchange:** higher net remittance per migrant, and less need for hundi (which is often used to repay informal migration debt).
- **Debt bondage reduction:** the mechanism through which most migrant exploitation operates.
- **Employment:** thousands of jobs in testing, training and language instruction.

### 13. Technology Required
Digital skills passport with verifiable credentials, biometric-linked worker registry (NID integration), employer portal, testing and language-assessment platforms, MFS-linked loan disbursement and repayment. This is a *credentials* problem, and verifiable-credential standards are now mature.

### 14. Government Role
- **Ministry of Expatriates' Welfare and Overseas Employment**; BMET; BOESL; Ministry of Foreign Affairs (MOU negotiation); NSDA (standards); Bangladesh Bank (migration finance rules).
- **Government:** negotiate corridor MOUs; own testing and certification; enforce fee caps; publish the price index.
- **Private:** training delivery, employer relationship management, finance.
- **PPP:** essential — the state cannot run employer relationships at scale.
- **Policy change:** mandatory employer-pays clauses in new bilateral MOUs; licensing reform tying agency licences to verified fee compliance.

### 15. Major Barriers
**Political economy is the barrier** — the recruitment intermediary chain is powerful and profitable. Also: destination-country cooperation (Bangladesh is a price-taker in most corridors), enforcement capacity, and competition from other origin countries willing to accept worse terms.

### 16. Difficulty of Implementation
**8/10.**

### 17. Opportunity Potential
**10/10.**

### 18. Why Now?
Remittance hit a record **USD 32.8bn in 2025** and formal-channel share rose sharply after the August 2024 political change disrupted hundi networks — demonstrating that the informal architecture around migration *can* be broken when the political conditions change. That window is open now and will not stay open.

### 19. First 12-Month Pilot
- **Location:** one corridor (Japan's Specified Skilled Worker route or Korea EPS expansion are the best candidates because employer-pays is culturally established), origin districts: Cumilla, Brahmanbaria, Chattogram.
- **Users:** 1,000–3,000 workers.
- **Partners:** MoEWOE/BMET, a destination-country employer federation, an NSDA-accredited training provider, a bank for migration finance, an ethical-recruitment certifier.
- **Budget [ASSUMPTION]:** Tk 15–30 crore including training infrastructure.
- **KPIs:** all-in cost per migrant (target <Tk 60,000); placement rate; wage achieved vs corridor average; loan repayment rate; 12-month retention in job.
- **Success:** median all-in worker cost below Tk 60,000 with ≥85% placement — publish the audited number, because the number itself is the political instrument.

### 20. OceanBlu / Entrepreneur Opportunity
Yes, and it is under-contested. Build first: an **ethical recruitment and skills-verification service for a single destination employer group** — not a mass agency. Sell verified, tested, language-ready workers to employers who need audit-proof supply chains, and charge the employer. First customer: a Japanese or Korean sector association, or a Gulf contractor working for an international principal with human-rights due-diligence obligations. Moat: the corridor MOU relationships, the verified-worker dataset, and an audited zero-fee track record — which competitors cannot fake. Scale: one corridor → several → become the certification standard other recruiters must buy.

---

## Opportunity #8 — A strategic health purchasing agency (national health protection scheme)

### 1. The Core Idea
Create a single public purchaser that buys defined healthcare packages from accredited public *and private* providers on behalf of enrolled households, paying by case-based rates with audited claims — rather than funding facilities by input budgets. Start with catastrophic inpatient cover for the poorest, then widen.

### 2. Bangladesh Problem
Gaps 8, 67. Out-of-pocket spending reached ~**79% in 2024** (BIDS), up from 73% in 2021 — one of the highest in the world. The poorest households spend ~**35% of income** on health versus 5% for the richest. Households spend on average **Tk 3,454/month** on health, ~11% of household expenditure. This is the largest single driver of impoverishment in Bangladesh. [VERIFIED]

### 3. International Benchmark
- **Thailand — Universal Coverage Scheme ("30-baht")**, National Health Security Office, **2001–02**: covers ~76% of the population, largely informal-sector.
- **India — Ayushman Bharat PM-JAY**, National Health Authority, **2018**: Rs 5 lakh cover per family.
- **Indonesia — JKN/BPJS Kesehatan (2014)**; **Rwanda — Mutuelles de Santé**.

### 4. Proof That It Works
- **PM-JAY:** **127 million (12.69 crore) hospital admissions authorised** as of 30 June 2026; **>Rs 1.92 lakh crore** of claims approved; **>42 crore people enrolled** (Oct 2025); the Indian Economic Survey 2024-25 credits it with saving families **>Rs 1.52 lakh crore** in out-of-pocket costs. [VERIFIED]
- **Thailand UCS:** operating since 2002, covering ~76% of the population in the informal sector, with a copayment of ~30 baht (~USD 0.90) later waived. [VERIFIED]

### 5. Bangladesh Current Situation
**Early-stage (B).** Bangladesh's **Shasthyo Suroksha Karmasuchi (SSK)** is a real, evaluated, government scheme: **Tk 50,000 annual cover per household** against a government-financed premium of **Tk 1,000**, piloted in three upazilas of Tangail covering ~**400,000 people in ~100,000 households**, with KfW support. Its evaluation is strong: SSK members using inpatient care had **92% lower out-of-pocket expenditure** and **72% lower incidence of catastrophic health expenditure** than comparison areas. [VERIFIED] The gap is not proof of concept — **Bangladesh has already proved the concept on its own population and then failed to scale it.**

### 6. The Bangladesh Opportunity
This is the strongest "proven at home, unscaled" case in the dossier. SSK's own evaluation results are better than most international schemes report. Bangladesh also has an unusually large, capable private hospital sector that is currently paid entirely in cash by patients — meaning a purchaser could contract real capacity immediately rather than waiting for public facilities to be built. And there is a hard fiscal argument: **USD ~5bn/yr already leaves the country for foreign hospitals** (Opp 41) — a domestic purchaser could redirect a share of that spending into domestic providers.

### 7. Localization
- **Purchaser, not insurer.** Do not attempt a contributory insurance model in an economy with a 6.56% tax/GDP ratio and 85% informal employment; tax-financed purchasing (Thailand's choice) is the only realistic architecture. Contributions can be layered later for formal-sector workers.
- **Buy from private providers from day one.** SSK's public-facility-only design is its main scaling constraint; India's private empanelment is what made PM-JAY scale.
- **Case-based payment with published rates and mandatory claim audit** — this is where Indian states learned expensive lessons about fraud.
- **Use NID + BDX (Opp 1) for enrolment and deduplication**, not a new card.
- **Start with a narrow, high-impact package**: maternal complications, injury/trauma, dialysis, cancer chemotherapy, and cardiac emergencies — the conditions that actually bankrupt households.
- **Fund it from a dedicated source** (a health surcharge on tobacco and/or a share of e-invoicing-driven VAT gains, Opp 4) so it is not hostage to annual budget negotiation.

### 8. Who Could Implement It?
**Government** (a statutory purchasing authority under MoHFW, modelled on India's NHA), with **private** claims processing, provider network management, fraud analytics, and hospital IT. Substantial commercial opportunity in the **third-party administration (TPA)** and claims-technology layer.

### 9. Business / Funding Model
**Tax-financed public purchasing**, with private vendors paid per claim processed. The private-sector business is TPA services, fraud analytics, provider credentialing, and hospital claims software — a large, recurring, B2G/B2B market that does not exist in Bangladesh today.

### 10. Target Users / Beneficiaries
- **Pays:** the Treasury (and later, formal-sector contributions).
- **Uses:** enrolled households, hospitals, claims processors.
- **Benefits:** the poorest households first; the private hospital sector (a new payer); the wider economy (medical impoverishment is a major poverty driver).

### 11. Estimated Market Potential
- **TAM [CALCULATED]:** Bangladesh's total health expenditure, of which ~79% is out-of-pocket. Households spending **Tk 3,454/month** across ~40m households [CALCULATED] implies household health spending on the order of **Tk 1.6 trillion/yr (~USD 13.6bn)**. That is the pool a purchaser would progressively displace.
- **SAM [CALCULATED]:** scaling SSK's own unit economics — Tk 1,000 premium per household — to 10 million poorest households costs **Tk 10bn/yr (USD 82m/yr)**, which is remarkably affordable and is the single most compelling arithmetic in this dossier. Even at a more realistic Tk 2,500–4,000 per household, 10m households costs Tk 25–40bn/yr.
- **SOM (private TPA/claims market) [CALCULATED]:** at 3–5% of claims value for administration, a Tk 25bn scheme supports **Tk 750m–1.25bn/yr** of private administration revenue.

### 12. Economic / Social Impact
- **Poverty:** the largest single lever available. SSK's own evaluation shows 92% lower OOP among inpatient users. [VERIFIED]
- **Foreign exchange:** retention of a share of the ~USD 5bn spent on treatment abroad.
- **Health system:** a purchaser creates the first real quality lever in Bangladeshi healthcare, because payment can be conditioned on accreditation.
- **Employment:** claims processing, provider auditing, hospital administration.

### 13. Technology Required
Beneficiary registry (NID-linked), claims adjudication engine, provider empanelment and credentialing system, fraud/anomaly detection, hospital-side claim submission software, and interoperability via BDX (Opp 1).

### 14. Government Role
- **Ministry of Health and Family Welfare**; Health Economics Unit (which already owns SSK); Finance Division; a new statutory purchasing authority.
- **Government:** legislate the purchaser; fund the premium; set rates; accredit providers.
- **Private:** deliver care; process claims; build systems.
- **PPP:** yes, on administration; the purchasing function itself must be public.
- **Policy change:** a National Health Protection Act creating the purchaser as a statutory body with ring-fenced financing.

### 15. Major Barriers
Fiscal space (the binding one — which is why Opp 4 is its precondition); provider fraud (universal in this model, manageable with audit); institutional resistance from facility-based budget holders; the political difficulty of choosing which package to cover first.

### 16. Difficulty of Implementation
**8/10.**

### 17. Opportunity Potential
**10/10.**

### 18. Why Now?
OOP spending is *rising* (73%→79%), the health budget share has been falling, and SSK's evaluation evidence is now published and positive. Meanwhile India's PM-JAY has de-risked the design at scale next door, and Bangladeshi patients' loss of easy access to Indian hospitals (visa restrictions cut Bangladeshi medical travel to India from ~500,000 in 2023 to ~482,000 in 2024) creates immediate domestic demand pressure. [VERIFIED]

### 19. First 12-Month Pilot
- **Location:** scale SSK from three Tangail upazilas to one full district plus one urban corporation area, and **add private provider empanelment** — the specific missing variable.
- **Users:** 250,000–500,000 households.
- **Partners:** HEU/MoHFW, KfW or another DFI, 10–20 private hospitals, a claims-technology vendor, an audit firm.
- **Budget [ASSUMPTION]:** Tk 60–150 crore/yr at that scale.
- **KPIs:** enrolment; claims per 1,000 enrolled; OOP reduction (repeat the existing evaluation design); claim rejection and fraud rates; average claim turnaround.
- **Success:** replicate the 92% OOP reduction result *with private providers in the network* and keep administrative cost under 6% of claims.

### 20. OceanBlu / Entrepreneur Opportunity
The purchaser must be public — but the **entire administration stack is a private market that does not yet exist in Bangladesh**. Build first: hospital-side **claims and empanelment software plus TPA services**, initially for the private insurance and corporate-health market (which exists today and is badly served), so the business is viable before any national scheme. First customers: private hospital chains and corporate health-benefit buyers. Moat: claims data, provider network relationships, and being the incumbent when a national scheme needs an administrator. Scale: corporate health → SSK district contracts → national TPA.

---

## Opportunity #9 — Single-window licensing plus a standing regulatory guillotine

### 1. The Core Idea
One digital front door for every business licence, permit, clearance and renewal — combined with a permanent institutional mechanism that inventories the regulatory stock, applies a cost-benefit test, and repeals or simplifies what fails. The platform is the visible half; the guillotine is the half that actually creates value.

### 2. Bangladesh Problem
Gaps 9, 14. Roughly **10 million MSMEs** contribute about **25% of GDP** but operate across a licensing landscape spread over dozens of agencies with independent statutes, no shared identifier, and no sunset review. [VERIFIED on MSME count and GDP share; ASSUMPTION on licensing fragmentation — BIDA's one-stop service exists but coverage is partial.]

### 3. International Benchmark
- **Singapore — GoBusiness / LicenceOne** (Ministry of Trade and Industry + GovTech), consolidating licence applications.
- **Korea — Regulatory Reform Committee** (1998): the original "regulatory guillotine", which reviewed the entire regulatory stock and abolished roughly half.
- **Rwanda — Irembo + Doing Business reform machinery** (2015–), the most relevant low-income precedent.
- **Croatia, Mexico, Kenya** — documented regulatory guillotine exercises.

### 4. Proof That It Works
Korea's 1998 guillotine is the canonical case: a systematic review of the national regulatory stock with a default-repeal rule, delivering large-scale simplification within roughly a year — the model subsequently exported by the World Bank/IFC to more than a dozen countries. Rwanda's Irembo demonstrates the digital-front-door half at national scale with a self-sustaining commission model (**>25m applications, ~USD 300m in transactions, >100m working hours saved**). [VERIFIED for Irembo; VERIFIED that the Korean guillotine occurred and was widely replicated — specific repeal percentages should be sourced from OECD regulatory policy reviews before quoting.]

### 5. Bangladesh Current Situation
**Underperforming (D).** BIDA operates a One Stop Service portal and Bangladesh has made periodic reform pushes, but the *stock* of regulation has never been systematically inventoried and pruned, and the front door does not cover most local-government and sector-regulator permits. [ASSUMPTION — verify BIDA OSS current agency coverage before investment.]

### 6. The Bangladesh Opportunity
LDC graduation in **November 2026** removes preference-based competitiveness and makes *domestic* cost-of-doing-business the residual lever. Bangladesh cannot change its wage advantage much; it can change its permitting friction quickly and cheaply. This is one of the few reforms with a fast, visible payoff that costs almost nothing.

### 7. Localization
- **The guillotine must be an institution, not an event.** Every country that ran a one-off exercise saw the stock regrow. Legislate a standing body with a default-repeal rule and a mandatory regulatory impact assessment for new rules.
- **Cover local government permits**, which is where SMEs actually experience friction (trade licence, signboard tax, fire, environment) and which national single-window projects habitually omit.
- **Give every business one identifier** across NBR, RJSC, city corporation and sector regulators — this is impossible without the BDX layer (Opp 1), which is why the two must be sequenced together.
- **Publish a public licence register**: which licences exist, what they cost, and how long they take. Transparency alone reduces informal payments.

### 8. Who Could Implement It?
**Government-led** (BIDA, Cabinet Division, Ministry of Commerce) with **PPP** delivery of the platform and a **consortium** (chambers of commerce + a research institute) doing the regulatory inventory.

### 9. Business / Funding Model
**B2G + transaction commission** on paid licence applications (Irembo model). Private opportunity: compliance-as-a-service for SMEs — a subscription that manages a firm's licences, renewals and filings.

### 10. Target Users / Beneficiaries
- **Pays:** businesses (fees/subscriptions); government (platform).
- **Uses:** MSMEs, corporate compliance teams, agency officials.
- **Benefits:** MSMEs; the tax base (formalisation); FDI.

### 11. Estimated Market Potential
- **TAM [ASSUMPTION]:** total licence and permit fee flow in Bangladesh is not published; do not invent it.
- **SAM [CALCULATED]:** compliance-as-a-service. If 100,000 formal SMEs pay Tk 12,000–30,000/yr for managed compliance → **Tk 1.2–3bn/yr (USD 10–25m/yr)**.
- **SOM [ASSUMPTION]:** Tk 150–400m/yr within 4 years.

### 12. Economic / Social Impact
Formalisation (which feeds Opp 4's tax base and Opp 44's credit market), investment climate, and reduced informal payments. The employment effect is indirect but broad.

### 13. Technology Required
Workflow/BPM platform, payment integration, e-signature, business identifier resolution, and a public regulatory register. Deliberately unglamorous.

### 14. Government Role
- **BIDA**, Cabinet Division, Ministry of Commerce, Local Government Division, RJSC, NBR.
- **Government:** mandate agency onboarding; legislate the guillotine and RIA requirement; enforce a "no licence outside the register" rule.
- **Private:** platform, integration, SME compliance services.
- **Policy change:** a Regulatory Reform Act; a business identifier mandate.

### 15. Major Barriers
Agency resistance (licences are revenue and leverage); local government autonomy; the guillotine's political sponsor requirement — this reform dies without sustained cabinet-level backing.

### 16. Difficulty of Implementation
**7/10.**

### 17. Opportunity Potential
**7/10.**

### 18. Why Now?
LDC graduation (Nov 2026) and the need to attract FDI into non-RMG sectors make cost-of-doing-business reform urgent and politically saleable.

### 19. First 12-Month Pilot
- **Location:** two sectors (light engineering and agro-processing) nationally, plus all licences in one city corporation.
- **Users:** 2,000–5,000 firms.
- **Partners:** BIDA, a city corporation, DCCI/FBCCI, a policy research institute.
- **Budget [ASSUMPTION]:** Tk 8–15 crore.
- **KPIs:** licences inventoried; % repealed or simplified; median days to licence; number of agency visits required.
- **Success:** a published regulatory register for the two sectors, ≥25% of requirements simplified or removed, and median licensing time halved.

### 20. OceanBlu / Entrepreneur Opportunity
The platform is a government contract; the durable business is **SME compliance-as-a-service**. Build first: a subscription that tracks and files every licence, renewal, VAT return and RJSC filing for small firms — a real pain point today with no reform required. First customers: fast-growing SMEs and foreign-invested SMEs who cannot navigate the system. Moat: process knowledge and agency relationships, plus accumulated filing history. Scale: compliance → accounting and payroll → SME lending distribution (Opp 44).

---

## Opportunity #10 — Individual learning accounts / a national skills credit

### 1. The Core Idea
Give every working-age adult a personal, government-funded training credit usable only with approved providers for approved courses, with outcomes published per course. Funding follows the learner, not the institution — which forces training providers to compete on employment outcomes rather than on budget allocation.

### 2. Bangladesh Problem
Gaps 10, 52, 60, 65. Bangladesh's training system is supply-driven: institutions are funded whether or not graduates get jobs, and employers do not trust the certificates. Meanwhile LDC graduation exposes up to **USD 8bn of annual export earnings** and a modelled **11.8% decline in RMG exports**, implying real displacement risk in the country's largest employer. [VERIFIED]

### 3. International Benchmark
- **Singapore — SkillsFuture Credit**, SkillsFuture Singapore, **2015–16**.
- **Indonesia — Kartu Prakerja**, Project Management Office under the Coordinating Ministry for Economic Affairs, **2020**: training vouchers + cash transfers delivered through a digital marketplace — the most transferable model because it was built for a large, informal, low-income, mobile-first population.
- **France — Compte Personnel de Formation (CPF)**, 2015.

### 4. Proof That It Works
- **SkillsFuture:** ~**1.05 million Singaporeans (~37% of the population)** have used their credits since 2016; **260,000 users in 2024**, up 35% from 192,000 in 2023; SSG-supported training rose from ~520,000 to ~555,000 learners; **69% of learners reported improved work performance** (up from 65%), **64% linked training to career advancement**, and **54% of Career Transition Programme participants found a job within six months**. [VERIFIED]
- **Kartu Prakerja:** peer-reviewed and J-PAL-registered evaluations find it **significantly increased the probability of employment among unemployed participants** and raised income — with the important caveat that **effects were concentrated in Java and urban areas and were insignificant in rural areas**. [VERIFIED — and this caveat is the single most important design input for Bangladesh.]

### 5. Bangladesh Current Situation
**Absent (A).** Bangladesh has NSDA, sector skills councils, TTCs and donor-funded skills projects — but no learner-held entitlement, no funding-follows-the-learner mechanism, and no published course-level employment outcomes. [ASSUMPTION — verify with NSDA; the absence of published outcome data is itself the diagnostic.]

### 6. The Bangladesh Opportunity
Bangladesh has the delivery rails Indonesia needed and had to build: **239.3m MFS accounts** and a national ID. Disbursing a training credit to 5 million people is operationally trivial here. What Bangladesh lacks — and what this creates — is a **market signal**: publish employment outcomes per course, and low-quality providers lose funding within two cycles. That single mechanism does more for TVET quality than a decade of institutional reform.

### 7. Localization
- **Learn from Prakerja's rural failure.** Rural effects were insignificant. So: restrict the initial credit to occupations with *verified* local demand, require providers to demonstrate employer placement partnerships, and pay providers partly on placement, not purely on enrolment.
- **Pay in tranches tied to completion and placement**, not upfront — the main fraud vector in voucher schemes.
- **Bundle a stipend**, as Prakerja did; a poor worker cannot attend training without income replacement, and this is what distinguishes a real programme from a symbolic one.
- **Prioritise migration-linked skills** (Opp 7) and care skills (Opps 31, 34, 40) where wage returns are highest and verifiable.
- **Publish outcomes publicly per provider** — this is the whole mechanism; without it, it is just another training budget.

### 8. Who Could Implement It?
**Government (NSDA, Ministry of Education/Ministry of Labour)** funding the credit; **private marketplace operator** running the platform, provider vetting and outcome tracking; **training providers** competing for learners; **employers** validating standards.

### 9. Business / Funding Model
Government-funded credit (public); the **platform operator earns a take-rate** on redeemed credits (Prakerja's structure), plus employer-paid recruitment fees for placements. Training providers earn per learner and per placement.

### 10. Target Users / Beneficiaries
- **Pays:** government (and later, an employer training levy).
- **Uses:** workers and jobseekers; training providers.
- **Benefits:** workers; employers (better-matched hires); the platform operator.

### 11. Estimated Market Potential
- **TAM [CALCULATED]:** 77.4m labour force. A credit of Tk 15,000 to 5% of the labour force per year (3.87m people) = **Tk 58bn/yr (USD 476m/yr)** of training expenditure created.
- **SAM [CALCULATED]:** platform take-rate at 3–6% of redeemed credits → **Tk 1.7–3.5bn/yr (USD 14–29m/yr)**; plus the training-provider market itself, which is the larger opportunity for operating companies.
- **SOM [ASSUMPTION]:** Tk 300–900m/yr for the platform operator at a 1m-learner scale.

### 12. Economic / Social Impact
Productivity and wages via better matching; resilience for RMG workers facing post-LDC adjustment; female participation if childcare-compatible delivery is designed in (Opp 34); and — uniquely — the creation of a **national labour market information asset** (gap 65) as a by-product of the transaction data.

### 13. Technology Required
Digital wallet/voucher tied to NID, MFS disbursement, provider marketplace, learning delivery (mobile-first, low-bandwidth, Bangla), outcome tracking linked to employment data. Nothing exotic; the difficulty is outcome verification, not delivery.

### 14. Government Role
- **NSDA**, Ministry of Education (TVET), Ministry of Labour and Employment, ICT Division, Finance Division.
- **Government:** fund the credit; set standards; publish outcomes; police fraud.
- **Private:** platform, training, placement.
- **PPP:** yes — Prakerja is explicitly a government-funded, privately-delivered marketplace.
- **Policy change:** a statutory training entitlement and a provider accreditation-with-outcomes regime.

### 15. Major Barriers
Fiscal cost (again pointing back to Opp 4); provider fraud and ghost enrolment — the dominant failure mode internationally; rural effectiveness (per Prakerja's own evidence); and institutional resistance from existing publicly funded training institutions that would lose guaranteed budgets.

### 16. Difficulty of Implementation
**7/10.**

### 17. Opportunity Potential
**8/10.**

### 18. Why Now?
LDC graduation is a scheduled, dated shock (24 November 2026) to the sector employing ~4 million people, most of them women. A displacement-response instrument needs to exist *before* the adjustment, not after. Meanwhile MFS penetration has made disbursement trivial for the first time.

### 19. First 12-Month Pilot
- **Location:** Gazipur, Narayanganj and Savar industrial belts (highest RMG concentration and highest displacement exposure).
- **Users:** 50,000–100,000 workers.
- **Partners:** NSDA, BGMEA/BKMEA, 20–40 vetted training providers, an MFS provider, an evaluation partner running a randomised design.
- **Budget [ASSUMPTION]:** Tk 90–160 crore including stipends (dominated by the credit value itself).
- **KPIs:** redemption rate; completion rate; employment/wage at 6 and 12 months versus a control group; cost per employed outcome.
- **Success:** a statistically credible employment effect and a published per-provider outcome table — the table is the durable institutional product, more than the pilot itself.

### 20. OceanBlu / Entrepreneur Opportunity
Two entries. The safer one: become a **high-outcome training provider** in a specific, verifiable, high-wage niche (overseas care work, industrial maintenance, welding to international codes, or CNC), and compete on published placement rates — a business that works with or without a national credit scheme. The more ambitious one: build the **marketplace and outcome-tracking platform** and sell it to NSDA. Build first: the provider business, because it generates the outcome data that makes you the credible platform operator later. First customer: an employer group (BGMEA members, or a Gulf/Japanese employer federation). Moat: verified placement outcomes and employer relationships. Scale: niche provider → multi-sector provider → national platform → export the platform to other South Asian countries.
