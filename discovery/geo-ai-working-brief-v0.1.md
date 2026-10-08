# Geo.ai: My Working Brief (v0.1, DRAFT)

**Status:** Private working draft, v0.1, started Thursday Oct 8, 2026. It is deliberately incomplete and is meant to hold my thinking as it develops. It's not for sending yet. Eventually I'll shape it into a note to Craig and Dave covering what I read, what I observed, and what I recommend.
**Voice:** Sections marked *(my thinking)* are mine. Sections marked *(tentative)* are starting positions I expect to change.
**Detail and citations:** `/workspace/geo-ai/exec-summary-v1.md`. Doc IDs below (0G, 13A, etc.) refer to the discovery packet's filename prefixes.

---

## TL;DR

- Craig and Dave have done months of serious domain thinking, but **the product, buyer and price are still undefined**. Craig's own Oct 4 brief says so (13A).
- **Most of the evidence is thin or AI-amplified.** There were six friendly conversations, none documented as recorded and none about price, against roughly 30–35 AI-generated assessments (exec summary §3).
- **This isn't white space.** Geoscience BC and Purple Rock bulk-indexed 43-101s with CSA permission (1), and AiMinr claims a 20,000+ report knowledge graph with benchmarking and due diligence (7H). Any edge has to come from something deeper, and nothing has shown that yet.
- **Nobody has tested the big technical and legal questions:** data rights, SEDAR+ access, extraction accuracy, and whether a well-prompted frontier model already does most of this.
- **My proposal:** a short, cheap experiment phase (about 3 weeks) funded by a small budget from Craig and Dave ($500–$1,000 in model and compute credits), with Gabriel and me supplying the technical work.
- **I'd want a cofounder role** (roughly CPO, hands-on). Roles, equity and Craig's position need settling before I put in serious hours.
- **I'll put the hard questions to them as "here's how I'm thinking about it"**, not as verdicts, and have Gabriel review first.

---

## What I read

- An 80-item discovery packet from Craig Banks (CB) and Dave Turner (DT), covering March to October 2026. It has 60 Word docs, 18 PDFs, 1 spreadsheet, and a Drive zip that turned out to be an exact duplicate.
- **Founder working sessions** (0A–0G, 6, 11): how the idea evolved, plus the 50/50 intent, the $1M indicative value and the plan to bring in Gabriel and me.
- **Six discovery conversations:** Sarah Caven (geologist and past 43-101 author), Jeremy Vincent (streaming side), Britt Blumell (GoldSpot background), NB at AMC (consultancy), Jeff Kyba (exploration geologist and author), and Don T. (mining-company project evaluation).
- **About 30–35 AI-generated docs:** assessments of interviews, competitors (7-series), TAM (7A1/7A2), concept recaps (8A–C), MVP mock-ups (6E2/6E3) and syntheses (10A–D).
- **Hard material:** Dave's 26-slide deck (4), the UBC MSc thesis on orebody knowledge flow (10), the Desharnais "Classification Debt" study of 200+ reports (6J1), the NI 43-101 instrument and Form F1, and 12 sample technical reports. The sample set is 3,767 pages and about 1.1M words, and every report has extractable text. There's also a page-count matrix mapping report sections for 8 of the reports.
- **Craig's Oct 4 brief to me** (13A) and his "Mining Project Development 101" primer (13B). These are the newest and most candid documents.

---

## Observations

**Strengths**
- The domain framing is strong. They understand the 43-101 regime, the QP role, report structure and the limits of a summary document (4, 9A, 13B).
- They are honest about their doubts. 0D (Apr 2) admits a lack of conviction, 0E defers personas to avoid biasing interviews, and 13A says "Be willing to tell us the idea is not ready."
- They reached credible people across relevant roles, and some signals line up. Report *writing* is a weak standalone product (JV, NB, Britt, JK, Don). Buyers need more than geology (JV, Don, JK). Comparing projects over time interests people (JK, Don).
- There is real raw material for experiments: the 12-report sample set, the page-count matrix, and the Desharnais study (strong evidence of extractable signal, and of how hard it is to extract).

**Gaps**
- None of the six conversations is documented as recorded. Two sets of notes were partly AI-written (6F1, 6H1).
- No one talked about price, budget or commitment. Every pricing number is an unsourced AI guess (7A1, 6E2, "1. commercial").
- The segments they called most promising (securities and exchange reviewers, bankers) were never interviewed (0E, 8C, 0F).
- No technical validation exists. There's no data-rights answer (flagged in 1 and 6, never resolved), no SEDAR+ access test, no extraction-accuracy test, and no frontier-model baseline. The only "POC" is a heuristic 1–10 scoring of 5 reports by one person (3).
- The 0G plan (manual pilot in September, company formation in October) appears not to have happened.

**Pivot history in brief**
- Mar: a 43-101 drafting tool, then a pre-submission review and "FICO score", then a "Bloomberg for mineral assets" for investors (0A, 0B, 3, 5).
- Apr: an "AI geologist" truth layer, then a 43-101 QA and benchmarking tool, then a tool for securities reviewers (0D, 8A–8C, 6E2, 0E).
- May–Jun: corporate memory, then an "Orebody Knowledge system of record", then ontology-as-IP and a "default platform for mining project intelligence" (6F1/6F2, 10A–10E, 0G).
- Oct 4: back to discovery, with "longitudinal records of mineral projects" and a proposed first experiment on 3–5 BC deposits (13A).
- The constant through all of it is 43-101s as the anchor, with expert-in-the-loop review as the claimed moat. The buyer changed about six times.

**Competitor reality**
- Prior art and adjacent players already exist. Geoscience BC, Purple Rock and Kildalton indexed 12,790 CSA-supplied reports with CSA permission (1). MiningHub does aggregation and screening (7D, 0D Apr 8). VRIFY does visualization and extraction (7G1/7G2). S&P is the data incumbent (7B). AlphaSense does document intelligence (7H).
- **AiMinr is the one to worry about.** It claims a knowledge graph from 20,000+ technical reports covering benchmarking, due diligence and compliance (7H, "Threat Level: High"). MinersAI targets analyst screening (7H).
- All of this competitor work is desk research from public positioning. Nobody has trialled these products.

**Bias in the AI-generated docs**
- The AI documents outnumber the evidence they interpret, and they consistently reframe lukewarm signals as validation. 6F1 says "Britt did not lean in"; 6F2 says the same conversation "materially upgraded" the concept.
- In the May 29 syntheses the concept score escalates from 7.5 to 8.5 to 9.0 (10C, 10D).
- 10B is DT's ChatGPT drawing on his own history, and the document itself is titled for "Bias".
- 6H1 was structured from a template derived from the Britt conversation.
- I'll treat the 0-series notes, the interview notes and 13A as the real record. I'll treat the AI docs as brainstorming.

---

## My current thinking *(my thinking)*

**1. A small budget, as skin in the game.**
I'll ask Craig and Dave for roughly **$500–$1,000 in model and compute credits** to prototype and answer the riskiest technical questions. The money is less important than the signal. It shows they're committed to testing the idea, not just discussing it, while Gabriel and I contribute the expertise. I'll tie the budget to a defined 3-week experiment with a written decision at the end (see "Proposed path").

**2. Roles. I'd want to be a cofounder.**
- **Me:** roughly Chief Product Officer, but doing a lot of hands-on product development, not just strategy.
- **Gabriel:** probably CTO.
- **Dave:** maybe COO or CEO. This is unsettled. 11 records Dave as comfortable mainly as advisor and domain expert. It also says his deeper involvement depends on Geo.ai keeping a broader social, environmental or economic purpose. 13A has him owning the domain model. So a CEO or COO title would mean a bigger commitment than he has signalled.
- **Craig: open question.** My thinking doesn't yet place him. That has to be addressed directly given three facts. Craig and Dave have a 50/50 intent and a ~$1M indicative value (6, 11). His Dingo employment may limit participation (0G). He plans about one day a week after roughly six months (11). His natural lane is commercial, strategy, partnerships and funding (0G, 13A §14).

**3. How I'll raise the big questions.**
I'll present the legal, structural and strategic questions as "here's how I'm thinking about it": a tentative view plus the evidence that would change it. I won't present them as conclusions. Gabriel reviews before anything goes to Craig and Dave. The aim is to invite pushback, not to win arguments.

---

## Big questions to push on *(each view is tentative)*

| Question | How I'm thinking about it *(tentative)* |
|---|---|
| **Data rights (SEDAR+ and CSA)** | Assume we can't commercialize a bulk corpus until counsel confirms we can. Purple Rock needed CSA permission (1). Small-scale research use for the experiment is probably lower risk, but I want that confirmed. |
| **Liability for scoring reports and QPs** | Start with tools that help people do their own review (gap-finding, comparison) rather than public scores or rankings of QPs. "Name and shame" and QP rankings (6/Apr 3, 0F, 6I1) look like defamation and negligent-misstatement risk. Needs counsel. |
| **Securities law and adviser registration** | Publishing project or issuer assessments to investors could raise adviser-registration questions (for example NI 31-103 in Canada, or US equivalents). This is my concern, not something the packet covers or I've verified. Ask counsel before building any investor-facing product. |
| **MNPI** | Any product that takes draft or pre-submission reports holds market-moving information. If we go there, plan security, access controls and insider-trading policy from day one (0E, 6E2). |
| **Structure and equity** | Settle this before I put serious hours in. The $1M indicative value (11) has no stated basis. The "contribution ledger" for unpaid work is vague. Nonprofit, PBC or incubator ideas (0G, 10E) don't fit naturally with founder equity. My lean: a for-profit with a stated public-benefit mission, with vesting for everyone. Very tentative. |
| **Craig's Dingo employment** | Counsel needs to read the actual IP-assignment and outside-activity terms before anything is formalized. If Craig is constrained, his role and equity should reflect that. I need to check my own employer constraints too. |
| **Who is the buyer?** | My current guess is project-evaluation and corporate-development teams at royalty/streaming companies and mid-tier miners, with consultancy QA leads as the alternative. Test both head-to-head. Desharnais (OR Royalties, 6J1) is the ideal first conversation because he compiled 200+ reports by hand. |
| **Willingness to pay** | We have zero evidence today. Each artifact interview should ask for a concrete commitment: a paid pilot, data sharing or an LOI. If the answer is just "interesting", treat it as a no (6E3's own test). |
| **Frontier-model baseline** | This is the most important technical question. If a well-prompted current model gives an expert most of the value on the 12 sample reports, the moat thesis shrinks. 13A asks exactly this. Run it first. |
| **Ontology vs lighter structure** | Start with a lightweight schema plus provenance (source, page, date; fact vs interpretation). Only formalize an ontology if the experiments show it adds something. The UBC GiM Map models information flow inside operating mines, not public disclosure (10). |

---

## Proposed path forward

**About 3 weeks, roughly matching exec summary §5.**
- **Week 1: ground rules and cheap tests.**
  - Working session with Craig and Dave. Agree roles, NDAs, IP assignment and the budget.
  - Start the SEDAR+ access spike and the frontier-model baseline on the 12 sample reports, with Dave blind-scoring outputs against 10–15 questions.
  - Book a short legal consult on data rights and liability.
  - Trial competitor products, starting with AiMinr, MinersAI and MiningHub.
  - Book 4–6 interviews.
- **Week 2: build artifacts.**
  - Reconstruct histories for 2 BC deposits (3–5 if tractable). Red Chris, Blackwater and Galore Creek are mentioned in 13B; Craig and Dave should choose.
  - Measure section and table extraction against the page-count matrix and a gold set Dave defines.
- **Week 3: test with users and decide.**
  - Run artifact interviews with willingness-to-pay asks.
  - Do a first-pass cost model.
  - Write a decision memo: define an MVP, run a narrower experiment, or stop.

**What $500–$1,000 buys *(ESTIMATE; check current model pricing before quoting)***

The basis is the sample set I measured: 12 reports, about 1.1M words, roughly **1.5M tokens in total, about 125k tokens per report**. For list pricing I've assumed a range of about **$2–$15 per million input tokens** and **$10–$75 per million output tokens** across mid-tier and top-tier models. These are assumptions, not quotes.

| Activity | Rough token volume (est.) | Rough cost (est.) |
|---|---|---|
| One full read of all 12 reports, plus structured summaries | ~1.5M in / ~0.6M out | ~$10–$70 |
| Frontier-model baseline: ~15 questions per report, full context each time, no caching | ~22M in / ~1M out | ~$55–$400 |
| Same baseline with prompt caching or retrieval | a fraction of the above | ~$20–$150 |
| Extraction evaluation: 30–50 fields × 12 reports × 2–3 models, 2–3 iterations | ~10–15M in | ~$30–$250 |
| Project histories: 3–5 deposits × ~5–10 reports each, ~3–5 passes | ~10–30M in | ~$30–$450 |
| PDF/table parsing tooling, mostly open-source | — | ~$0–$100 |

**Bottom line (estimate):** $500 likely covers a disciplined 3-week experiment if we use caching or retrieval and mid-tier models for bulk passes. $1,000 gives headroom for top-tier models on the expert-facing comparisons. The bigger costs are our time and Dave's expert-review hours, not compute.

---

## Open questions

**For Craig and Dave**
1. If you had to bet on one paying buyer today, who is it?
2. Will you fund the $500–$1,000 experiment budget, and who approves the spend?
3. Craig: what do your Dingo terms allow for IP, outside work and non-compete? What role do you see for yourself if Gabriel and I join as cofounders?
4. Dave: how much time can you commit, and would you want an operating role (COO or CEO), or stay as domain lead?
5. Is the 50/50 agreement signed? What's the basis for the $1M figure, and how would the contribution ledger convert to equity?
6. Has anyone looked into SEDAR+ or CSA reuse rights, or asked Purple Rock or Geoscience BC how they got permission?
7. Are there raw notes or recordings for the interviews, especially Britt (6F1) and Don (6I1)?
8. Did the September manual pilot or the ontology work start (0G)?
9. Which 3–5 BC deposits should we use, and can Dave commit review hours in the next 3 weeks?
10. Would any interviewee be a design partner, or pay for a manual review now?

**For me**
1. How many hours a week can I realistically give, and for how long?
2. Do I have any employer conflict or IP-assignment constraint?
3. What cofounder terms would I accept (equity, vesting, credit for unpaid work)?
4. When should Gabriel come in: now, or after the baseline results?
5. Am I willing to contribute toward the budget myself if they don't fund it, or is their funding a deliberate test of commitment?

---

## TODO / to fill in

- [ ] **[Scott]** My view on the right buyer after reading more. Placeholder.
- [ ] **[Scott]** My proposed equity and vesting framework. Placeholder.
- [ ] **[Scott]** What I think Craig's role should be. Placeholder.
- [ ] **[Scott]** Run the deep-research prompts below and fold in the findings.
- [ ] **[Gabriel]** Review the technical plan and the "here's how I'm thinking" framing.
- [ ] Confirm current model pricing and update the budget table.
- [ ] Draft the legal question list for counsel (data rights, liability, adviser registration, MNPI, Dingo terms).
- [ ] Decide what goes in the eventual note to Craig and Dave, and the tone.
- [ ] Pick a decision date for after the 3-week experiment.

---

## Appendix A: Deep-research prompts (paste-ready)

Each prompt is self-contained. Run them separately in a deep-research tool.

### Prompt 1: Data rights, regulatory and legal exposure

> **Context:** I'm evaluating a startup concept ("Geo.ai") that would build an AI-structured, longitudinal database of Canadian NI 43-101 mineral-project technical reports (filed on SEDAR+), linked to other public disclosures, stock and commodity price history, and expert interpretation. Possible products include benchmarking and gap analysis of technical reports, project-maturity assessment, due-diligence screening for royalty/streaming companies and miners, and possibly pre-submission review of draft reports. Earlier research found that Geoscience BC, Purple Rock and Kildalton obtained permission from the Canadian Securities Administrators (CSA) to build a full-text database of NI 43-101 reports. The CSA reportedly provided 12,790 reports (~1.9M pages) filed up to September 2019, and 996 BC-related reports were linked to the BC MINFILE database.
>
> **Research questions:**
> 1. What do the current SEDAR+ terms of use say about automated access, bulk download, storage, and commercial reuse of filed documents? Are there official bulk-data or licensing programs?
> 2. What exactly did the Geoscience BC / Purple Rock / Kildalton permission cover (scope, terms, commercial vs public use)? Are there other precedents of CSA or provincial regulators licensing filings to third parties?
> 3. Who holds copyright in NI 43-101 technical reports (issuer, consulting firm, QP)? How do report disclaimers about third-party reliance affect a third party analyzing or redistributing them? What fair-dealing (Canada) and fair-use (US) considerations apply to text-and-data mining and to displaying excerpts?
> 4. If a company publishes scores, rankings or "red flags" about technical reports, projects, issuers or named Qualified Persons, what defamation, negligent-misstatement and product-liability exposure does it face in Canada and the US? How do analogous businesses (credit rating agencies, ESG raters, research providers) manage it?
> 5. Could selling project or issuer assessments to investors require registration as an adviser under Canadian securities law (e.g., NI 31-103 and its exemptions) or the US Investment Advisers Act (including the publisher exclusion)? What design choices reduce that risk?
> 6. What obligations arise from handling unreleased draft technical reports (material non-public information): insider-trading and tipping rules, confidentiality, security expectations?
> 7. What is the status of the CSA's 2025 proposal to repeal and replace NI 43-101, and what would it change for report structure or machine-readability?
>
> **Output:** A memo with (a) an executive summary of the top 5 risks ranked by severity and likelihood, (b) a section per question with findings and primary-source citations (regulator pages, instruments, case law, terms of use), (c) a table of design mitigations, and (d) a list of specific questions to take to Canadian securities counsel. Flag clearly where evidence is missing or ambiguous. Do not guess.

### Prompt 2: Competitive reality, and whether frontier models already do this

> **Context:** Geo.ai would analyze NI 43-101 (and eventually JORC and S-K 1300) mining technical reports. It would extract and normalize key parameters, benchmark reports against peers by deposit type and stage, flag gaps, inconsistencies and unsupported assumptions, and track how a project's technical understanding changes across successive reports. The claimed differentiation is a deeper, expert-reviewed reasoning layer about project maturity and what's missing, beyond aggregation and search. I need to know whether that space is already occupied, and whether general-purpose frontier LLMs already do it well enough.
>
> **Part A: competitors.** For each of AiMinr, MinersAI (including "MinersAI Analyst"), MiningHub, VRIFY (including VRIFY Signal), S&P Global Market Intelligence (metals and mining), AlphaSense, EarthLabs/GoldSpot, Mining Data Online, Purple Rock and OneMine, plus any other relevant companies you find (especially new AI startups from 2024–2026), report:
> - The product and target users.
> - Data sources and claimed corpus size. AiMinr reportedly claims a knowledge graph built from 20,000+ technical reports. Verify it.
> - Whether they extract structured data from technical reports, benchmark reports or projects, detect gaps or deficiencies, or track projects over time.
> - Pricing, if public.
> - Funding, team size, notable customers and partnerships.
> - Evidence quality: marketing claims vs demos vs customer testimony.
>
> **Part B: frontier-model capability.** What is the current evidence (papers, benchmarks, vendor case studies, practitioner write-ups) on LLM performance for long technical PDFs (100–600 pages) with dense tables and figures? Focus on (1) field-level extraction accuracy from tables, (2) section segmentation, (3) cross-document comparison, and (4) mining or geoscience reports specifically, including any published experiments on NI 43-101, JORC or S-K 1300 documents. What are the known failure modes (table parsing, unit normalization, hallucination, implicit parameters such as drill spacing that are rarely stated explicitly)?
>
> **Output:** (a) A competitor comparison table, with columns for extraction, benchmarking, gap detection, longitudinal tracking, target buyer, pricing, funding, and evidence quality. (b) A one-paragraph threat assessment per company. (c) A "white space" analysis: what, if anything, is not being done. (d) A frontier-model capability summary with citations and a recommended evaluation design for testing a model on a 12-report sample set. Cite sources, mark unverified claims, and do not speculate beyond the evidence.

### Prompt 3: Buyer economics (royalty/streaming, miners, consultancies, regulators)

> **Context:** Geo.ai is exploring who would pay for AI-assisted analysis of NI 43-101 mining technical reports. Candidate buyers:
> - (1) Project-evaluation and technical due-diligence teams at royalty and streaming companies (e.g., Wheaton Precious Metals, Franco-Nevada, Royal Gold, OR Royalties, Triple Flag).
> - (2) Corporate-development and technical-services teams at mid-tier and major miners.
> - (3) Consulting firms that author reports (e.g., SRK, SLR, SGS, Tetra Tech, WSP, AMC, Ausenco), for QA and review efficiency.
> - (4) Securities and exchange reviewers (BCSC, OSC, TSX/TSXV).
> - (5) Mining-focused bankers and investors.
>
> Early interviews suggested that streamers receive deals mainly through bankers rather than scanning filings themselves. They also suggested consultancies rely on templates and past reports rather than AI platforms, and that buyers need engineering, metallurgy, ESG and economic analysis, not just geology. A 2019 source cited TSX as having 1 dedicated technical reviewer and TSXV 3. A count of early-2026 SEDAR+ filings annualizes to roughly 600–700 NI 43-101 technical reports per year on SEDAR+.
>
> **Research questions:**
> 1. For each buyer type: how is technical review done today (team size, process, tools)? What does it cost in time and money (for example, cost of a technical due-diligence review, cost to produce a PEA, PFS or FS report, internal QA time)? Who owns the budget? How are software tools procured?
> 2. What evidence exists on the frequency and types of deficiencies in NI 43-101 reports (CSA staff notices, regulator review reports, compliance actions, restatements, retractions)?
> 3. How many NI 43-101 technical reports are filed per year (last 5 years) by type (MRE, PEA, PFS, FS), and what share do the large consultancies author?
> 4. What do adjacent tools charge these buyers (mining data subscriptions, document-intelligence platforms, technical-review services), as pricing anchors?
> 5. What publicly documented failures (for example, resource write-downs after production) show the financial cost of missed technical risk? Include the scale of losses where available.
>
> **Output:** (a) A buyer-by-buyer profile table covering workflow, pain, budget owner, likely willingness to pay with evidence, and sales cycle. (b) A ranked recommendation of the best 1–2 beachhead segments, with reasoning. (c) Filing-volume and authorship data with sources. (d) Pricing anchors. (e) Gaps in public evidence that require primary interviews, with 5 suggested interview questions per segment. Cite sources and distinguish evidence from inference.

---

## Appendix B: Pointer

Full analysis, document inventory, claims-vs-evidence table and the complete feasibility task list (A1–A8, B1–B10, C1–C12) are in **`/workspace/geo-ai/exec-summary-v1.md`**. Extracted packet text is in `/workspace/geo-ai/extracted/`.
