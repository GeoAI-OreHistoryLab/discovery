# Geo.ai: Executive Summary of the Discovery Packet (v1)

Prepared by Geo.ai Product Lead for Scott Cressman · October 7, 2026
Source: `/Users/scottcressman/Development/geo-ai/discovery/from-banks` (80 items), copied to the box. Extracted text for every document is saved in `/workspace/geo-ai/extracted/`. Document IDs below (0G, 6F2, and so on) are the filename prefixes.

**Who's who (from the documents):** CB is **Craig Banks**: commercial lead and author of 13A/13B. He works at "Dingo" (0G), and 0G describes him as your "long-time trusted colleague". DT is **Dave Turner** (also written David Turner): geologist and domain lead, author of the 4 deck and most interview notes. **Gabriel** is an AI architect reached through you (0G, 11). Craig and Dave treat the idea as a **50/50 joint venture** (6, 11).

---

## Headline takeaways

1. **This is a well-framed problem looking for a product.** Over seven months the team has convinced itself that mining project knowledge is fragmented, hard to compare and dependent on experts. It has not chosen a buyer, a wedge or a price. Craig's latest brief to you says so directly: the product is "not yet... sufficiently defined to simply start building an MVP" (13A, Oct 4, 2026).
2. **The concept pivoted about eight times between mid-March and late June (about 15 weeks).** It went from a 43-101 drafting tool to a pre-submission review and "FICO score", then an investor "Bloomberg for mineral assets", an "AI geologist" or truth engine, a 43-101 QA and benchmarking tool, a securities-reviewer tool, a corporate-memory system, an "Orebody Knowledge system of record", and finally a "longitudinal record of mineral projects" (dates in §1). One thing stayed constant: NI 43-101 reports as the anchor dataset, with expert human-in-the-loop review as the claimed moat.
3. **The primary evidence is thin.** There were 6 conversations with industry people (Sarah Caven, Jeremy Vincent, Britt Blumell, NB at AMC, Jeff Kyba, Don T.). None is documented as recorded and none asked about price. No regulator, exchange reviewer or banker was interviewed, even though those groups were named as the most promising buyers (0E, 8C). Roughly half of the 60 Word docs are AI-generated assessments of that small evidence base, and they read as increasingly self-reinforcing. In 10C and 10D, both dated May 29, an AI scores the concept 7.5, then 8.5, then 9.0 out of 10.
4. **The "nobody does this" claim does not hold.** The packet's own research shows Geoscience BC and Purple Rock bulk-indexed 12,790 CSA-supplied 43-101s, with CSA permission (1). It also describes **AiMinr** as having a knowledge graph built from more than 20,000 technical reports, offering benchmarking, due diligence and compliance (7H, rated "Threat Level: High"). MinersAI targets investment screening (7H) and MiningHub covers aggregation (0D Apr 8, 7D). Any claimed differentiation now rests on a deeper reasoning and "project progression" layer that hasn't been demonstrated.
5. **No technical feasibility work exists yet, and that is your assignment.** Nobody has tested data rights, SEDAR+ acquisition, extraction accuracy, or a frontier-model baseline. Section 9 of 13A asks you two questions: can we create the intelligence, and can we obtain and structure the data at reasonable cost? The 12 sample reports in folder 3 (3,767 pages, about 1.1M words, all with extractable text) are a ready-made test bed.
6. **Business-formation issues are live and unresolved.** Craig's Dingo employment may limit his participation (0G). Neither founder can go full-time (11). There is an indicative $1M internal value and a proposed "contribution ledger" for your and Gabriel's unpaid work (11). The team is also weighing nonprofit, PBC or incubator structures (0G, 10E) that are hard to square with founder equity. These need settling before you put significant hours in.
7. **The best next step is a narrow, falsifiable experiment, not an MVP.** 13A proposes reconstructing the full histories of 3–5 BC deposits, and it sets a guardrail: "If a well-prompted frontier model can produce substantially the same value, we should know that now." I agree. I'd run that alongside a frontier-model baseline and a data-rights check, then put the artifacts in front of 3–5 of the people already interviewed, with explicit willingness-to-pay questions (§5).

---

## 1. The idea

### Current best articulation (from 13A, Oct 4, 2026, the newest document)

Geo.ai would build a **structured, evidence-linked, longitudinal record of mineral projects**. The backbone is about 25 years of NI 43-101 technical reports, which give successive standardized snapshots of the same deposit. The team wants to link those with other disclosures (news releases, resource updates, studies, assessment reports, permitting, ownership and financing events), market data (stock and commodity prices) and expert-reviewed interpretation. The aim is to represent "what is known about a mineral project, how confidently it is known, how that understanding has changed, what remains unresolved, and how that project is progressing relative to comparable projects" (13A §3).

Several products could sit on top of that record. 13A lists them as context, not commitments: project screening and diligence, project progression and maturity, benchmarking, exploration intelligence, historical project reassessment, and technical review and QA. The near-term wedge that recurs most often is an **NI 43-101 assessment and benchmarking tool**: find gaps, inconsistencies and missing work against a peer corpus, and assess project maturity (0E, 0F, 6G1, 10C, 11).

- **Who it serves:** still open. Candidates include consultants and QPs writing reports, mining companies (corporate development, technical services), securities and exchange reviewers, streamers, royalty companies and banks, retail investors, governments and First Nations (6, 0D Apr 8, 6H1, 13A §12).
- **The problem:** 43-101s are standardized in format but not in judgment. They are long, hard to compare across projects and over time, vary in quality, and are only summaries of the underlying work. Investment and development decisions rest on expert reading that doesn't scale (9A, 6C, 13A §2).
- **The claimed moat:** linked historical project records, a structured mining-domain framework (the "ontology", perhaps seeded by the UBC GiM Map), expert-reviewed interpretation, and links between evidence, progression and outcomes (13A §7, 10E). 13A explicitly asks you to challenge whether frontier models make this unnecessary.

### Trajectory of pivots

| Date | Doc(s) | Framing | What triggered it |
|---|---|---|---|
| Mar 10/13 | 0A | Look for lifecycle bottlenecks. AI drafts 43-101s from a data room ("90–98% complete"), re-analyzes historical reports against a "gold standard", builds a Canadian deposit knowledge base. | Founders' first conversation. The filename says Mar 10, the body says Mar 13. |
| Mar 13 | 0B | "AI Mining Intelligence Platform anchored in NI 43-101": pre-submission review and ranking tool for issuers and exchanges, a "FICO score" for projects and reports, the database as the long-term asset. Horizons 1–3. | Drafting judged too heavy (an "IT and data-cleaning business"). |
| Mar 17 | 3 | Craig solo: reject report writing. Build "decision intelligence" by normalizing assumptions across reports. H1 captures data via mining companies; H2 is an investor platform, a "Bloomberg Terminal for mineral assets". Heuristic 4-pillar scoring of 5 reports. | Reading the sample reports. |
| Mar 19–23 | 4, 0C, 5, 6 | Dave's deck: report taxonomy, filing triggers, decision tree, workflow entry (pre-submission build and review, exchange review tool), "reviewers likely overloaded". 5 defines an "AI-powered mining asset intelligence platform... translation layer between geology and capital markets". 6 decides to validate before building, run interviews, and set 50/50 ownership. | Deck plus consolidation. |
| ~early Apr | 5B, 8A, 0D (Apr 2) | "AI geologist": first-principles, deposit-specific reasoning, and a "domain truth layer" deciding what is actually true about a deposit. Start with orogenic gold or Cordilleran Cu-Au porphyries. Financial institutions are seen as the most likely buyers. | Lack of conviction. Worry that a few consultancies (SRK, Golder, Hatch) write most reports, so a writer or reviewer tool has a small market. |
| Apr 8 | 0D (Apr 8), 8B, 7D | Three-layer stack: data (MiningHub, S&P), reasoning, decision/truth. Interpretation, not aggregation. "Truth audits" on porphyry copper as an MVP. QP reputation scoring. | Discovering MiningHub. |
| Apr 15–20 | 6/JV notes, 6E1, 6E2, 6E3, 0E, 8C, 9A–9C | "43-101 QA & Benchmarking Tool" (consultants first, then mining companies, then investors). Then securities and exchange reviewers as the most promising niche. New framing: "Improve the quality, credibility, and comparability of technical disclosures before they reach capital markets." Stock and commodity prices become co-anchors (9B). | Jeremy Vincent said streamers like Wheaton get deals through bankers and don't scan 43-101s, and that geology alone isn't enough. |
| ~late Apr–May | 6F1, 6F2 | "Corporate memory loss" as the wedge: capture decision context during exploration. Pitched as "a continuously learning geological intelligence system". | Britt Blumell conversation. Britt "did not lean in" on benchmarking (6F1). |
| May 13–31 | 6/NB notes, 6G1, 6G2 | "Technical report intelligence and benchmarking layer", not a generator. Consultants as partners and early adopters. | AMC uses templates and past reports, with no unified AI platform. |
| May 28–29 | 10A–10D, 0F | Orebody Knowledge (OBK): "Orebody Knowledge Maturity Platform", "system of record for Orebody Knowledge", a project "heat map" and maturity score. Horizons run up to "mining project digital twins". | UBC GiM Map thesis. |
| Jun 18–26 | 6H1/6H2, 6I1, 0G, 10E | Historical reinterpretation ("geological hindsight engine"), a mine-development (not just geology) model, people as a dataset. The ontology becomes the primary IP. Nonprofit, PBC or incubator considered. Manual pilot on 20–30 projects. Vision: "default platform for mining project intelligence". You are brought in for technical feasibility. | Jeff Kyba and Don T. conversations. Craig's employment constraints. |
| Undated (after 0G) | 11 | Neither founder can go full-time, so you and Gabriel would build. MVP is still an NI 43-101 assessment or advisory tool. 50/50 founder agreement, ~$1M indicative value, NDAs, target early 2027 (Roundup/PDAC). | Capacity. |
| Oct 4 | 13A, 13B | Step back: "still in discovery". Longitudinal project records. First experiment: 3–5 BC deposit histories. Guardrails. You are asked to say whether this is ready. | Brief for you. |

Note that the "system of record" framing came from AI synthesis on May 29 (10D). 13A, which is newer, is more cautious. It warns against equating mine development with technical quality and against "prematurely build[ing] a model that predicts which deposits become mines" (13A §5).

---

## 2. What was in the discovery packet

There are 80 items: 60 .docx, 18 PDFs, 1 .xlsx and 1 zip (macOS `._*` files ignored). The total size is about 386 MB.

**The zip adds nothing new.** `Discovery (General Visibilty)-20261007T192554Z-1-001.zip` is a Google Drive export containing 79 files. I compared it with the loose files by filename and MD5: all 79 are byte-identical, and nothing exists only in the zip or only in the loose folder.

### A. Founder working sessions (CB + DT): primary record of their thinking
- **0A** (Mar 10/13): AI in geology, bottlenecks, the 43-101 drafting idea, Purple Rock, a Canadian deposit knowledge base.
- **0B** (Mar 13): 43-101 as the anchor, pre-submission review and ranking, "FICO score", assessment reports as the next data layer, Horizons 1–3, possible advisor Andy Fagan.
- **0C** (Mar 20): summary of Dave's deck (4): taxonomy, data layers (primary, adjacent, distal), workflow entry points, multi-sided use cases.
- **6** (Mar 23): validate before building, 5-slide engagement deck, stakeholder list, moat questions, legal and data-usage risk, 50/50 JV.
- **0D** (Apr 2): consultant concentration, return to "AI geologist" plus human-in-the-loop, financial institutions as buyers, start with porphyry or orogenic gold.
- **0D** (Apr 8): MiningHub reframes the idea as a three-layer stack, possible MiningHub partnership ("nervous system" vs "brain"), QP reputation.
- **0E** (Apr 20): debrief of the Jeremy Vincent conversation. Bankers originate deals. Section-by-section benchmarking. Securities and exchange reviewers as a niche. Pre-submission per-review pricing idea. Contact Vicky Yeh.
- **0F** (May 29): UBC thesis, OBK node framework, project heat map, QP ranking, pre-submission assessment as the strongest near-term opportunity. Actions include researching rejection rates (no output from this appears in the packet).
- **0G** (Jun 26): move from ideation to company planning. Your role and Gabriel's. Ontology as the main IP. Nonprofit, PBC or incubator. Manual POC on 20–30 projects. Founder roles. July–October timeline.
- **11** (undated, after 0G): commitment levels, bringing in you and Gabriel, 50/50 agreement, ~$1M indicative value, contribution ledger, NDAs, early-2027 target.

### B. Discovery interviews: primary evidence
- **6/2026 04 03 Friendly Discovery Conversation 1**: Sarah Caven (Vancouver geologist, past 43-101 author, works on responsible sourcing; CDL minerals stream per 0D) with Dave, Apr 3, not recorded. Topics: gaps in reports, a "better than SEDAR" interface, QP matchmaking, "name and shame", garbage-in/garbage-out risk. Dave flags her bias.
- **6/2026 04 15 Notes from in-person Discovery with JV**: Jeremy Vincent (streaming/royalty side; "Jeremy at Wheaton" per 6B). Covers how due diligence works (bankers run the process, then NDA, data room, high-level screen, deep diligence). "Geology alone would not be enough". How do you define "good"? 43-101s are incomplete by design. Saw value in a high-level diligence tool.
- **6/2026 05 12 NI43101_AI_Workflow_Conversation_Notes_David_Turner**: NB from AMC with Dave, May 13. AMC works from section templates and past reports, with no unified AI platform. Skeptical of automated report writing. Sees value in benchmarking and QA against a corpus. Also does JORC and S-K 1300 work.
- **6F1**: Britt Blumell (GoldSpot background), Vancouver, not recorded, undated. Notes were "captured via dictation – and AI writing with inference". Benchmarking drew no pull ("Britt did not lean in"). Corporate memory loss was the strongest signal.
- **6H1**: Jeff Kyba (JK) with Dave, Jun 18. Values comparing projects over time and reinterpreting legacy data. Says AI should augment, not replace. Social and permitting constraints matter. Regulators as a possible user. The notes say the summary is "biased on a feed document... from Britt B".
- **6I1** (first part): "Don T." (likely Don Tollery, named in 0F), a mining industry evaluation professional, with Craig. Mentions AlphaSense and AiMinr. Large miners still use spreadsheets, disclosures and networks. People and management quality matter. Interested in ranking and economic translation. His employer isn't stated; the AI section mentions "(Barrick)" and "(Wheaton)" in passing.

### C. AI assessments of those interviews
**6D** (Sarah), **6E1** (JV), **6F2** (Britt), **6G1** and **6G2** (AMC), **6H2** (JK), the second half of **6I1** (Don, plus a founder skills table naming Craig, Dave, Scott/Gabe and Don), **6J2** (Desharnais article; "GEOAI relevance score 9/10").

### D. Discovery planning
- **6B**: stakeholder grid with about 25 named contacts across 10 segments, each marked "Friendly #1/#2". Regulators and communities have almost no names.
- **6C**: structured discovery guide (objective, problem, hypothesis, question bank by persona, assumptions).

### E. Concept, MVP and strategy documents (mostly AI-drafted)
- **1. problem space**: fact-check. Geoscience BC, Purple Rock and Kildalton got CSA permission and 12,790 reports (~1.9M pages); 996 were BC-related and linked to MINFILE. Reuse rights flagged as a constraint.
- **1. commercial areas**: four opportunities ranked. Pricing guesses of $25k–$250k/yr, unsourced.
- **1. Extension**: a reprinted a16z newsletter by Bobby Samuels (Protege DataLab) on the "data gap" and "FICO scores for AI data". Inspiration only, not about mining.
- **2. Market timing**: critical-minerals policy push, 20 years of digital disclosure, LLM readiness.
- **2. Competitive landscape**: aggregators, geo-software, exploration AI, internal bank databases, general AI platforms.
- **2. Three Versions of the Pitch**: one-liners for executives, AI people and investors.
- **3. 43-101 POC**: Craig's solo session (Mar 17). Heuristic 4-pillar scores (Economics, Confidence, Stage, Optionality) for 5 assets: Detour 8.6, Rainy River 7.7, 3Ts 5.1, Gold Terra 4.8, Sitka 4.5. Explicitly "heuristic scoring, not model-driven".
- **4. NI43101 Leveraging** (26-slide deck by Dave Turner, V001 Mar 19 / V002 Mar 20): thesis, report categories A–G, decision-tree workflow, early products by report stage and customer type, data layers, filing triggers, single- vs multi-author patterns. Slide 9 counts SEDAR+ filings: **Jan 48, Feb 51, Mar 1–20 44**. It also cites a 2019 source saying TSX had 1 dedicated technical reviewer and TSXV had 3. A cursory review of 30 recent reports found one with obvious deficiencies (budget mismatch, chapter order, maps without north arrows).
- **5. High Level Overview**: 4-phase plan (structuring, scoring, upstream QA, portfolio intelligence). "Turn any 43-101 into a decision-ready investment summary in minutes."
- **5B**: first-principles "AI geologist" moat. 10–20 AI-assisted expert evaluations before any software. Lists failure modes for orogenic gold and porphyry deposits.
- **6E2**: MVP 1 "43-101 QA & Benchmarking Tool". Consultants first ("produce ~70%+ of reports"), pricing $2k–$10k per report or $25k–$100k per firm per year. All unsourced.
- **6E3**: text mock-up of the MVP 1 UI in Consultant and Owner modes. All numbers are illustrative (for example "92% of comparable PEA reports include all three"), not data.
- **8A, 8B, 8C**: concept recaps (truth layer, porphyry "truth audits" MVP, shift to disclosure quality and regulators).
- **9A, 9B, 9C**: Craig's AI-assisted research (Apr 20). 43-101 history (Bre-X, 1998/2001, 2005, 2011, CSA 2025 repeal-and-replace proposal), stock and commodity prices as co-anchors, a document taxonomy beyond 43-101. 9A says ~800 reports/yr could not be verified.
- **10A–10E**: UBC thesis assessment. **10B** is DT's ChatGPT response; the title flags "Bias" and the answer draws on DT's earlier chats (hyperspectral, "Live Update Pipeline Template"). **10C** and **10D** are AI syntheses with escalating scores. **10E** is the Jun 26 vision statement.
- **13A**: Product Thesis & Build Guardrails v0.3 (Craig, Oct 4), written for you. **13B**: Mining Project Development 101 (Craig, Oct 4). Covers stages, resource vs reserve, deposit vs project vs company, date semantics (examples: Red Chris, Blackwater, Galore Creek).

### F. Market sizing and competitors (all AI desk research, no primary data)
- **7A1** TAM: 600–1,000 reports per year, 7,000–13,000 "high-value" users, and the claim that 25% share at $1k/yr is $1.75–3.25M ARR. A global extension gives 15,000–30,000 users and "$2.55–10.5M", which doesn't follow from its own inputs (15–30k × 25% × $1k = $3.75–7.5M).
- **7A2** volume: 400–800 per year globally (300–600 on SEDAR), a "high-value" subset of 150–300, and 8,000–15,000 historically.
- **7B** S&P Global, **7C** FirstPrinciples, **7D** MiningHub, **7E** SRK internal tools (likelihood percentages with no basis), **7F** EarthLabs, **7G1** VRIFY, **7G2** VRIFY Signal (quotes Steve de Jong), **7H** AlphaSense, MinersAI, AiMinr.

### G. External and reference material
- **6J1**: Guy Desharnais (VP Project Evaluation, OR Royalties), "Classification Debt" (Jun 16, 2026). He compiled drill spacing by hand from more than 200 NI 43-101s (2022–2024). Operating mines need 3.6× (lower-continuity deposits) and 2.8× (higher-continuity) more drilling than development projects for Indicated resources. Of 43 Canadian Au/Ag mines built since 2015, 18 (42%) underperformed on head grade. He notes that drill spacing is "rarely stated explicitly" in reports. **This is the best evidence in the packet that valuable signal exists in 43-101s and that extracting it is hard.**
- **10**: UBC MSc thesis, Carolina Marín Suárez, "Mapping Geological Information Flow in the Mining Value Chain" (March 2026, 164 pp; supervisor Shaun Barker). The GiM Map has 505 information nodes and 2,786 directed connections, for flotation-based porphyry copper systems. It finds that information-integration barriers are mainly organizational and cultural. Limitations: ordinal weights, and no modeling of uncertainty propagation or decision criticality yet. Future work includes VoI/Monte Carlo and dynamic decision support. **Caveat:** the map covers information flow inside operating mines, not public disclosure. Using it as a 43-101 scoring ontology is a leap the packet doesn't test.
- **Folder 3 (43-101 Training Set):** 12 sample technical reports (catalogued below), the NI 43-101 instrument (consolidated to Jun 9, 2023), Form 43-101F1, Larsen et al. 2016 ("Minimum engineering requirements for assessing mining projects": PEA/PFS/FS expectations from a lender's view), a 1-page GiM Map poster misleadingly named like the thesis, and **43101PageCounts.xlsx**. That spreadsheet maps physical page counts to F1 items 1–30 for 8 reports. MRE-only reports carry one-page "not applicable" placeholders for items 15–22. Item 14 (resources) ranges from 22 to 105 pages, and item 16 (mining methods) from 1 to 87 pages.

**Sample report catalogue.** Only 12 are actual technical reports, not ~18 as briefed. Folder 3 holds 17 files in total.

| Issuer / project | Commodity | Author | Type | Effective date | Pages |
|---|---|---|---|---|---|
| Sitka Gold: RC Gold, Yukon | Au | GeoSim (independent, 1 QP) | MRE (early) | Jan 2025 | 114 |
| Kirkland Lake Gold: Detour Lake, ON | Au | Internal QPs | Operating mine TR | Jul 2021 | 406 |
| New Gold: Rainy River, ON | Au | Internal QPs | Operating mine TR | Dec 2024 | 235 |
| Gold Terra: Yellowknife City, NWT | Au | SGS | Updated MRE | Mar 2021 | 232 |
| Independence Gold: 3Ts, BC | Au-Ag | SGS | MRE update | Nov 2025 | 132 |
| New Found Gold: Queensway, NL | Au | SLR (+Stantec) | PEA | Jun 2025 | 465 |
| Heliostar: Goldstrike, Utah | Au | SLR | MRE | Mar 2026 | 259 |
| West Red Lake Gold: Madsen/PureGold, ON | Au | SRK | Updated MRE | Dec 2021 (signed Jun 2023) | 186 |
| Calibre: Pan, Nevada | Au | SRK (+APEX) | Resources & reserves update | Dec 2022 | 313 |
| Fission Uranium: PLS, SK | U | Tetra Tech | Feasibility study | Jan 2023 | 402 |
| Giga Metals: Turnagain, BC | Ni | Tetra Tech et al. | PFS | Sep 2023 | 440 |
| New Found Gold: Hammerdown, NL | Au | WSP (11 QPs) | PEA | Feb 2026 | 583 |

**What these reports are for:** a small, deliberately varied training and test set. The folders are organized by author firm (independent, internal, SGS, SLR, SRK, Tetra Tech, WSP), and the set spans the report types from early MRE to FS and operating mine. Five were used in the Mar 17 scoring POC (3). Eight were used for the page-count structure analysis (xlsx). Hammerdown appears in the deck (4). The set is 10 of 12 gold, includes only one porphyry-adjacent BC project (Turnagain is nickel), and contains no Cu-Au porphyry report, although porphyries are the repeatedly preferred starting domain (0D, 5B, 8B). The full catalogue is in `extracted/3. 43-101 Training Set/CATALOGUE.md`.

---

## 3. How deeply it has been researched and thought about

### What's strong
- **Domain framing is good.** The founders understand the 43-101 regime: triggers, report categories, the QP role, F1 structure, summary-vs-truth limits, deposit vs project vs company, date semantics (4, 9A, 13B). Dave's deck and 13B are solid primers.
- **They are genuinely self-critical.** They admit lack of conviction (0D Apr 2). They defer persona narratives so interviews aren't biased (0E). Dave notes interviewee bias (Sarah, 6/Apr 3). They repeatedly warn about scope creep. 13A in particular is an unusually honest brief: "We should distinguish evidence that the problem is real from evidence that GeoAI is the right solution" (13A §6), and "Be willing to tell us the idea is not ready."
- **They talked to credible people.** The six conversations cover distinct, relevant roles: early-stage QP, streamer/royalty investor, mining-tech operator, consultancy report author (AMC), exploration geologist and author, and mining-company project evaluator. Some signals converge across them: report writing is a weak standalone product (JV, NB, Britt, JK, Don); AI should augment experts (JK, Don, JV); geology alone isn't enough for buyers (JV, Don, JK); comparing projects over time is interesting (JK, Don).
- **There are useful hard artifacts.** The page-count matrix, the filing-rate counts (4, slide 9), the Desharnais study (6J1) and the 12-report sample set.

### What's thin
- **Volume and depth of primary evidence.** There are 6 conversations, most with "friendly" contacts (6B labels them that way). None is documented as recorded; Sarah's and Britt's notes explicitly say they weren't. Two sets of notes were partly AI-written: 6F1 by "AI writing with inference", and 6H1 structured from a Britt-derived template. Follow-ups with Andy Fagan were planned (0B, 0E) but no notes exist. The 6B contacts Drew Barr, Kendra Johnston, Matt Larkin and others have no notes in the packet either.
- **The segments called most promising were never interviewed.** That includes securities and exchange reviewers (0E, 8C: "most credible early users"; deferred in 0F), bankers (0E), mid-tier consultants (7A2's "best entry"), retail investors, and communities or First Nations.
- **No willingness-to-pay evidence.** No interview records a price, a budget, a buyer's procurement path, or a commitment such as a pilot, LOI or design partnership. Every price in the packet ($1k/seat in 7A1; $2k–$10k per report in 6E2; $25k–$250k/yr in "1. commercial") is AI-generated and unsourced. 13A concedes discovery "does not yet validate a specific product, buyer or willingness to pay."
- **No technical validation.** No SEDAR+ acquisition test, no extraction accuracy measurement, no frontier-model baseline, no data-rights or legal review (flagged as a risk in 1 and 6, never resolved), and no outcome dataset. The only "POC" (3) is a heuristic 1–10 scoring of 5 reports by one person, with no ground truth. The 0G plan (manual pilot of 20–30 projects in September, company formation in October) doesn't appear to have happened. By Oct 4, 13A still describes the project as discovery.
- **Competitor analysis is desk-only.** It's based on public positioning, and nobody trialled AiMinr, MinersAI, MiningHub, VRIFY Signal or AlphaSense. The distinctions drawn ("benchmarking vs validation", "mining intelligence vs orebody intelligence", 7H) are assertions. Some are circular: "If SRK already had this... you would have heard about it" (7E).
- **Market sizing is guesswork.** 7A1 and 7A2 are AI estimates with ±25–50% error bands and no sources.

### AI-generated vs primary
By my classification of the 60 Word documents:
- **About 10 founder meeting notes.** These are primary but probably AI-summarized from conversations: 0A–0G, 6, 11.
- **6 interview records.** Two are partly AI-written.
- **4 founder-authored framing docs.** 4, 6B, 6C, 13A/13B.
- **3 external pieces.** 1. Extension, 6J1, and the thesis (a PDF).
- **Everything else, about 30–35 docs, is AI-generated assessment, synthesis, competitor writeups, TAM, recaps or MVP mock-ups.** Examples: 1, 2-series, 5B, 6D, 6E1–3, 6F2, 6G1–2, 6H2, 6I1 part 2, 6J2, the 7-series, 8A–C, 9A–C, 10A–D.

The AI documents greatly outnumber the evidence they interpret. They also tend to reframe each interview as validation, even when the interviewee was lukewarm (compare 6F1's "Britt did not lean in" with 6F2's "The conversation materially upgraded the GEO.AI concept").

### Are the key claims backed?
| Claim | Backing in packet | Verdict |
|---|---|---|
| ~600–1,000 43-101s per year | Deck counts 143 filings from Jan 1 to Mar 20, 2026 (about 600–700/yr annualized). 7A1 says 600–1,000, 7A2 says 300–600 on SEDAR, 9A says "~800" unverified. | Roughly 600–700/yr on SEDAR+ is the only measured figure. Needs a proper pull. |
| Historical corpus of 8k–15k | 1 cites 12,790 reports supplied by CSA to Sep 2019 (Geoscience BC). AiMinr claims more than 20k across codes (7H). | Plausible order of magnitude. Not measured for SEDAR+. |
| Consultants write 60–80% of reports | 7A1 / 6E2 / 7A2, all unsourced. Internal contradiction: "top firms 40–60%" vs "consultants 70–80%". | Unverified. Cheap to measure from QP certificates. |
| No one does this / clear gap | Contradicted by 1 (Geoscience BC/Purple Rock), 7H (AiMinr, MinersAI), 0D Apr 8 (MiningHub). | Overstated. The gap, if any, is above aggregation and benchmarking, and it's unproven. |
| Reviewers overloaded / deficiencies slip through | Deck slide 9 (2019: TSX 1 reviewer, TSXV 3) and one anecdotal deficient report. Rejection-rate research assigned in 0F, never done. | Suggestive, not established. |
| Buyers will pay | No primary evidence. | Unbacked. |
| 43-101s contain learnable signal on outcomes | 6J1 (human compilation, 200+ reports) supports it, with caveats about extraction ambiguity. | Partially backed. Best evidence in the packet. |
| An ontology/OBK framework creates a moat | 10A–10E, AI reasoning only. The thesis is about internal mine information flow. | Hypothesis. 13A rightly asks you to test it. |

### Internal contradictions and unresolved questions
- **Who is the buyer?** Candidates have included investors (5, 0D Apr 2, "1. commercial"), consultants (6E2, 6G1), regulators and exchanges (0E, 8C), report authors and mining companies (10C), exploration teams via corporate memory (6F1), and finally "open" (13A). 0D Apr 2 says the consultant market may be "a handful of enterprises". Two weeks later, 6E2 makes consultants the primary buyer.
- **Predicting success.** 0B (FICO score), 10E ("probability this project becomes a successful mine") and 6J2 propose outcome prediction. 13A warns against equating mine development with quality.
- **Issuer-side vs investor-side.** 7F and 7G1 argue serving both sides "will be difficult". 6E2 and 6E3 sell the "same product, two sides".
- **Legal structure vs equity.** Nonprofit, PBC or incubator (0G, 10E) vs a $1M internal value and equity ledger (11) vs "not settled" (13A).
- **Data rights.** Flagged in Mar (1, 6) and again in 13A §9. No answer anywhere.
- **Smaller inconsistencies.** 0A's filename date doesn't match its body. 10C says the concept started "six months ago" when it was about 2.5 months. 7A1 has an arithmetic error. The 7-series layer taxonomies disagree on where VRIFY and MiningHub sit (7G1 vs 7G2 vs 7H).

### Signals of bias
- **AI sycophancy and escalation.** Concept scores go 7.5 → 8.5 → 9.0 within the May 29 syntheses (10C, 10D). One assessment says "This is exactly how your Dingo instincts apply" (6F1). Nearly every interview is labeled "validation, not redirection" (6H2, 6I1).
- **10B is explicitly labeled for bias.** It is DT's ChatGPT, which draws on his earlier conversations and agrees with his framing.
- **Template contamination.** 6H1's summary was structured from Britt's feed document.
- **Sample bias.** Interviewees are friends and trusted contacts (6B) who were shown the concept. That's appropriate early on, but it tends to produce encouragement rather than disconfirmation.
- **Interviewee bias.** Noted for Sarah (responsible sourcing).

### Overall rating
- **Problem understanding and domain framing: 7/10.** Strong, experienced, honest about limits.
- **Market and customer validation: 3/10.** A handful of friendly conversations with no recordings on file, no pricing, no target-buyer segment interviewed, and desk-only competition and TAM work.
- **Technical feasibility: 1/10.** Not started, by design. It's your remit.
- **Business formation readiness: 2/10.** 50/50 intent, but structure, roles, time commitment and employment conflicts are unresolved.

**Overall: about 3.5/10 on evidence, about 7/10 on thinking quality.** This is a thoughtful problem-exploration phase that has produced a lot of AI-amplified narrative but very little that could falsify the idea. It's at the stage where cheap, decisive experiments are worth more than more synthesis. 13A says the same.

---

## 4. Feasibility evaluation tasks

Priority key: **Now** means the next 2–3 weeks. **Next** means 1–2 months. **Later** means after a go decision. **[ENG]** marks a task best handed to a separate engineering bot.

### (a) Go-to-market and customer/market validation

| # | Task | Why it matters | Evidence that answers it | Priority |
|---|---|---|---|---|
| A1 | Pick 2 candidate beachhead buyers and test them head-to-head. My suggestion: (i) project evaluation and corporate development at royalty/streaming companies and mid-tier miners; (ii) consultancy QA leads. | The buyer has changed about six times. Nothing else can be prioritized until it's fixed. | 8–12 structured interviews per segment. Ask about the current workflow, time and cost of the task, who owns the budget, and what they'd pay. Ask for a commitment (pilot, data-sharing, LOI). | Now |
| A2 | Re-engage existing contacts (JV, Don T., Jeff Kyba, NB/AMC, Britt) with a concrete artifact (see C1/C2) rather than a concept. | 11 and 13A already plan this. Reactions to an artifact are far more informative than reactions to an idea. | Ratings of usefulness vs their current method, specific "would you use or pay for this on your next deal or report" answers, and requests for more. | Now→Next |
| A3 | Interview Guy Desharnais (OR Royalties, 6J1). | He compiled 200+ reports by hand: direct evidence of the manual pain and of extractable signal. He's an ideal design partner and a test of the royalty segment. | Did he try tools? What would he pay to have that compilation automated and kept current? | Now |
| A4 | Interview 2–3 securities or exchange reviewers (BCSC, OSC, TSX/TSXV), current or former, starting with Vicky Yeh (0E). | Called the most credible early users (0E, 8C) but never contacted. They also know deficiency patterns, which would make good benchmark labels. | Their review workflow, the deficiency frequency and taxonomy, attitude to AI pre-screening, procurement reality. Also check whether CSA staff notices or review reports publish common deficiencies (not in packet). | Next |
| A5 | Hands-on competitor teardown: AiMinr, MinersAI, MiningHub, VRIFY Signal, AlphaSense, S&P (trial or demo). | 7H rates AiMinr "High" threat with a 20k-report graph doing benchmarking, due diligence and compliance. Positioning claims are untested. | Feature-by-feature comparison on the same 2–3 sample reports. What they extract, whether they flag gaps or compare across time. Pricing. | Now |
| A6 | Measure the market inputs: annual SEDAR+ technical-report filings by type, author-firm share (from QP certificates), distribution of issuer stages. | TAM, consultant concentration and segment sizing are all unverified (7A1/7A2 contradict each other). | A filing-count dataset for the last 3–5 years. Pairs with B4/C3. | Next |
| A7 | Concierge pilot: sell or deliver 2–3 manual, AI-assisted project reviews or histories to real users. | The fastest way to test willingness to pay and output value before building (5B and 0G proposed similar ideas). | Whether anyone pays or commits time, and what they actually use. | Next |
| A8 | Positioning and messaging test once a buyer is chosen (avoid "grading", per 6E2's own risk note). | Being seen as a judge of QPs creates trust and liability friction. | Reactions to 2–3 framings in interviews. | Later |

### (b) Startup formation and business

| # | Task | Why it matters | Evidence that answers it | Priority |
|---|---|---|---|---|
| B1 | Define your role and terms before deep work: advisor, cofounder or contractor; time commitment; how unpaid contribution converts to equity (11's "contribution ledger"); vesting. | 11 proposes notional valuation of your and Gabriel's unpaid work against a ~$1M indicative value. That basis is arbitrary and the terms are undefined. | A written term sheet or MOU among Craig, Dave, you and (optionally) Gabriel. | Now |
| B2 | Clarify Craig's Dingo employment constraints and any IP-assignment or non-compete clauses. Check your own employer's policies too (not covered in the packet). | 0G says Dingo obligations create uncertainty about Craig participating, and drive the nonprofit idea. An IP-assignment problem could taint ownership. | Review of employment agreements by counsel. | Now |
| B3 | Execute the founder agreement, NDAs and IP assignment of work to date. | 11's 50/50 agreement and NDAs are planned. Packet docs and interview notes are the IP. | Signed documents. | Now |
| B4 | Data rights and licensing: SEDAR+ terms of use, CSA permission, copyright held by report authors and issuers, and the terms of any market-data source. | Purple Rock "obtained legal permission from the CSA" (1). Report disclaimers (for example SRK's on Pan) limit third-party reliance. Without rights, the core asset can't be commercialized. Flagged in 1 and 6, never resolved. | A lawyer's memo, plus an informal approach to CSA/BCSC about precedent. **[ENG]** for the technical side of access (rate limits, robots, bulk options). | Now |
| B5 | Liability and securities-law exposure of scoring reports, projects or QPs. | QP "name and shame" (6/Apr 3), QP rankings (0F, 6I1) and "independent red flags" (6E3) risk defamation or negligent-misstatement claims. Publishing project or issuer assessments to investors may raise adviser-registration questions under Canadian securities law (for example NI 31-103) or US equivalents. I haven't verified this; it is not in the packet and needs counsel. | Counsel's view. Product framing and disclaimers designed accordingly. | Next |
| B6 | Handling material non-public information (MNPI). | The pre-submission and draft-upload products (0E, 6E2, 0B) would hold unreleased, market-moving technical data. That creates insider-trading, security and confidentiality obligations. | Policy and architecture requirements (feeds C9). | Next |
| B7 | Choose a structure: for-profit, PBC, nonprofit or incubator. | 0G and 10E favor nonprofit or PBC for trust and grants. That conflicts with founder equity (11) and with IP ownership questions 0G itself raises. | Comparison of options against funding sources and founder goals. 0G assigned Dave to research this; no output in the packet. | Next |
| B8 | Funding path: grants (Geoscience BC precedent in 1; 0A and 0B mention government critical-minerals programs; none researched), angels (Alex Cervinka and others in 6B), customer-funded pilots. | Neither founder can go full time (11). Somebody has to fund your and Gabriel's time or an engineering budget. | A shortlist of programs with eligibility. My candidates to check (not in packet): IRAP, SR&ED, Mitacs, provincial programs. | Next |
| B9 | Business model and pricing hypotheses tied to the chosen buyer: per-report, seat or enterprise. | Current numbers are AI guesses spanning two orders of magnitude. | Pricing questions in A1 and the A7 pilot outcomes. | Next |
| B10 | Team gaps: mining engineer or evaluator (Don T. suggested in 6I1), time commitments, fractional CFO (0G). | The domain team is part-time and geology-heavy. JV and Don say buyers need engineering and economics too. | Commitments from named people. | Later |

### (c) Technical and engineering feasibility (mostly [ENG])

| # | Task | Why it matters | Evidence that answers it | Priority |
|---|---|---|---|---|
| C1 | **Frontier-model baseline** on the 12 sample reports. Ask the questions in 13A §2 and §10 ("what's missing?", "what changed between reports?", "how does this compare?") using only well-prompted current models with long context or retrieval. Have Dave blind-score the outputs. **[ENG]** + Dave | 13A's key guardrail. If baseline models deliver most of the value, the moat thesis collapses or narrows. | Expert-rated quality, error types, hallucination rate, cost per report. | Now |
| C2 | **Project-history experiment** (13A §10): pick 3–5 BC deposits with rich histories. Candidates from the packet are Red Chris, Blackwater and Galore Creek (13B); Dave and Craig should choose. Assemble every technical report and key disclosure, build an evidence-linked timeline, and test whether it helps a knowledgeable user. **[ENG]** + Dave | It tests the core hypothesis at small scale, and it's the artifact for A2. | Time and cost per project. What was automatable vs manual. User rating vs their current method. | Now→Next |
| C3 | Data acquisition spike: what is programmatically obtainable from SEDAR+ (current and legacy SEDAR archive), with what metadata and at what rate. Also check alternate sources (company websites; BC ARIS/MINFILE per 1; Nevada NBMG list per 1). **[ENG]** | 13A §9: "Can we realistically obtain and structure the data?" Ties to B4. | Coverage %, effort, blockers, an estimate of total corpus size. | Now |
| C4 | Parsing large PDFs. The sample reports run 114–583 pages and 4–34 MB. Tasks: segment each into F1 items 1–27 (which 43101PageCounts.xlsx gives as ground truth for 8 reports); extract tables (resources, costs, recoveries) and figures; handle placeholders and appendices; handle scanned legacy reports. **[ENG]** | Benchmarking depends on reliable section and table extraction. Some of the most important parameters live in tables or are only implicit (Desharnais: drill spacing "rarely stated explicitly"). | Section-segmentation accuracy against the xlsx. Table-extraction F1 on a hand-labeled set. Failure catalogue. | Now→Next |
| C5 | Extraction accuracy evaluation. Dave defines a 30–50 field schema (for example resource tonnage, grade and class by category; cut-off; metal price; recovery; capex/opex; NPV/IRR; drill spacing; study type; effective vs report date; QPs and firms). Build a gold set on the 12 reports and measure field-level precision and recall. **[ENG]** + Dave | Trustworthy structured data is the prerequisite for any comparison. 13A requires facts and inferences to stay distinguishable. | Per-field accuracy, confidence calibration, human review time per report. | Next |
| C6 | Benchmarking methodology: define peer groups (deposit type × stage × jurisdiction), normalization (common metal price, units), "completeness vs peers" metrics, and above all **what "good" means** (JV's challenge). Candidate labels: regulator deficiency letters, later restatements, Desharnais-style reconciliation outcomes. **[ENG]** + Dave | Without ground truth, scores are opinions (3's POC was heuristic). Small peer groups make statistics fragile (7A2 claims 50–150 per segment is enough, without support). | A written methodology, a pilot on one segment, and expert agreement rates (inter-rater). | Next |
| C7 | Entity resolution and longitudinal linking: deposit vs project vs company, ownership changes, renamed properties, multiple date types (13B: Red Chris amended and restated in 2015 with a 2012 effective date). **[ENG]** | 13A §9 lists this explicitly. Longitudinal records fail without stable IDs. | Linking accuracy on the C2 deposits. | Next |
| C8 | Knowledge representation: compare a formal ontology or knowledge graph against a lighter schema plus retrieval. Decide whether to seed from the GiM Map (505 nodes / 2,786 edges, built for operating porphyry Cu mines). Design provenance so every assertion links to source, page and date, tagged as fact, interpretation or inference. **[ENG]** | 13A §8 asks you to challenge whether a formal ontology is needed at all. The "system of record" claim depends on provenance. | A prototype on C2 data. Can it answer the 13A §10 questions better than C1's baseline? | Next |
| C9 | Architecture sketch for a system of record: ingestion, document store, extraction pipeline, knowledge store, eval harness, expert review UI, tenancy and MNPI isolation for private uploads (B6). **[ENG]** | 0G asks you what architecture should underpin it. That should come after C1–C5 show what's needed. | Architecture decision record and a build-vs-buy list. | Later |
| C10 | Expert-in-the-loop design: what experts review, how corrections are captured as reusable data, the cost of an expert-hour, and how the cold-start problem is handled. **[ENG]** + Dave | It's the claimed moat in nearly every document. Nobody has tested whether experts will contribute (the 6C assumption "Are suitable experts willing to contribute knowledge?"). | Review-time measurements in C2 and C5, and expert willingness. | Next |
| C11 | Cost model at 10 / 100 / 1,000 / 10,000 projects (13A §9): compute, LLM tokens, storage, human review, data licensing. **[ENG]** | 13A asks where the hard part is: finding, extracting, linking, validating or reasoning. | A spreadsheet driven by C3–C5 measurements. My back-of-envelope from the sample: about 90k words (~125k tokens) per report on average, so ingesting ~600–700 new reports a year is modest. Human review is the likely dominant cost. | Next |
| C12 | Market and outcome data: sources and licensing for historical stock prices, commodity prices and corporate events (9B, 13A §5). **[ENG]** | Needed for outcome linking. Licensing can be expensive. | Source shortlist with costs and terms. | Later |

---

## 5. Key open questions and recommended next 2–3 weeks

### Questions for you (Scott)
1. What role do you want: advisor, technical cofounder, or paid builder? How many hours a week, for how long?
2. Do you have any employer conflict or IP-assignment constraint of your own? (The packet doesn't cover this.)
3. Should Gabriel be involved now, or only after C1–C3 produce results?
4. What budget, if any, is available for API, compute and data costs during the experiments, and who funds it?
5. Do you agree with treating the 13A brief (Oct 4) as the source of truth, superseding 10E's "default platform" vision?

### Questions for Craig (CB), and Dave where relevant
1. If you had to bet today on one paying buyer for the first product, who is it and why?
2. What exactly do your Dingo employment terms permit, including IP assignment, outside activities and non-compete?
3. Is the 50/50 founder agreement signed? What is the $1M indicative value based on, and how would the contribution ledger work for Scott and Gabriel?
4. Has anyone researched SEDAR+ or CSA reuse rights since the March flags (1, 6)? Has anyone contacted Purple Rock or Geoscience BC about their CSA permission?
5. Are there recordings, transcripts or raw notes for the interviews, especially Britt (6F1) and Don (6I1)? When was the Britt interview, and who led it?
6. What happened with the planned contacts: Andy Fagan, Drew Barr, Vicky Yeh, Kathleen Hanley, Kendra Johnston?
7. Did the September manual pilot (0G) or Dave's ontology ideation begin? Any outputs?
8. Which 3–5 BC deposits would you pick for the 13A experiment, and can Dave commit expert hours to scoring outputs over the next 3 weeks?
9. Would any interviewee act as a design partner, or pay for a manual review today?
10. Dave's continued involvement depends on a broader social, environmental or economic purpose (11). How should that constrain the first product?

### Recommended plan (about 3 weeks)

**Week 1: set the ground rules and start the cheap tests**
- A working session with Craig and Dave on the 13A questions. Settle B1–B3: your role, NDAs, IP assignment, and Craig's Dingo constraints.
- **[ENG]** Start C3 (SEDAR+ access spike) and C1 (frontier-model baseline on the 12 sample reports). Dave defines 10–15 test questions and a blind scoring rubric.
- Start B4: a short legal consult on data rights and liability, with a scoped question list.
- Start A5: competitor trials, prioritizing AiMinr, MinersAI and MiningHub.
- Line up 4–6 interviews for weeks 2–3: JV, Don T., Jeff Kyba, NB/AMC, Guy Desharnais, plus one securities reviewer.

**Week 2: build the artifacts**
- **[ENG]** C2: reconstruct histories for 2 BC deposits (expand to 3–5 if tractable), with C4 and C5 run on those reports plus the 12-report set. Measure manual vs automated effort.
- Read out C1 results. Is the baseline already "good enough" on summarization and gap-finding? Where does it fail (comparison over time, cross-project, missing-work detection)?
- Draft the interview guide around the artifacts, with explicit willingness-to-pay and commitment questions (A1, A2).

**Week 3: test with users and decide**
- Run 4–6 artifact interviews.
- **[ENG]** First-pass cost model (C11) and an architecture sketch outline (C9).
- Write a decision memo: proceed to a defined MVP, run another narrower experiment, or stop. Base it on three things: (1) is there intelligence beyond baseline models, (2) is the data feasible and licensable, and (3) has at least one segment shown real pull?

**What would change my view:**
- **Positive:** Dave rates the C2 histories clearly better than C1's baseline; at least two interviewees offer a paid pilot or data partnership; legal confirms a workable rights path.
- **Negative:** frontier models match most of the value; SEDAR+ bulk use is restricted without a licence; or no segment commits beyond "interesting" (6E3's own test: "'Interesting' → you lose").

---

*Working files on the box: per-document text in `/workspace/geo-ai/extracted/` (includes the 12 sample reports, the thesis, the deck and a CSV of the page-count matrix); training-set catalogue at `/workspace/geo-ai/extracted/3. 43-101 Training Set/CATALOGUE.md`; the unzipped Drive export in `/workspace/geo-ai/scratch/zip/` (identical to the loose files).*
