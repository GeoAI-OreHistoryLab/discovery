# Geo.ai: Platform Capabilities & Demo Narratives (v0.1)

**Status:** Working draft for Craig/Dave review and build targeting.  
**Sources:** Oct 16, 2026 Scott–Craig call (`scratchpad/banks-scott-oct-16.md`), `exec-summary-v1.md`, `geo-ai-working-brief-v0.1.md`, 13A/13B.  
**Purpose:** Prioritized capabilities for a thin-slice prototype, plus killer demo scripts for the ~10–15 discovery contacts and conference positioning.

---

## Prototype intent (from Oct 16)

- **Not** production software. Something that **looks and behaves like a product** on a **thin data slice**, with real enough plumbing to test feasibility.
- **Primary GTM use:** Short-circuit discovery—show the same **10–15 people** from round one a prototype, get feedback and willingness-to-pay signals, then sharpen (Craig: three rounds → two with a prototype).
- **Build rhythm:** Sprint with **Craig** first; **Dave** for alpha; broader network for beta. Craig may fund tokens (~$500+); Craig owns compartmentalized accounts (GitHub, model/compute, shared Geo workspace).
- **North stars mentioned on the call:** BC-focused corpus over time; major Vancouver mining conference (abstract/paper as forcing function); optional adjacency to VRIFY-style visualization exits—not chosen yet.

---

## Platform architecture (Craig’s four layers)

| Layer | What it is | Thin-slice stance |
|------|------------|-------------------|
| **1. Data platform** | Public sources assembled around **NI 43-101 as spine**: reports, issuer/company, QPs/firms, press releases, stock/commodity context. Entity resolution and longitudinal linking. Storage “amenable to AI.” | **Build first.** Moat vs frontier models (fragmented names, incomplete histories). |
| **2. Progression framework** | Simplified mine-development path (GiM / UBC thesis item 10): ~10–15 major steps, not 190. “How far along” vs known trajectories—not mine prediction. | **Demo-worthy P2.** Does not need to be fully accurate day one. |
| **3. First-principles geology** | Deposit-type reasoning, belt context, historical government/academic reports layered on the record. | **Defer** from first slice; “trickier… we’ll see.” |
| **4. Human in the loop** | Experts correct extractions/interpretations; corrections persist and improve downstream views. | **One polished loop** in prototype (Dave/associates later at scale). |

**Guardrails (13A + working brief):** Prefer gap-finding, comparison, and maturity **readings**. Avoid public **QP rankings**, **FICO-style scores**, and **“will this become a mine”** predictions in v0 demos. Craig still mentions QP/FICO on the call—if used at all, keep **internal/workflow**, not marketing.

---

## (a) Platform capabilities — prioritized

Priority reflects: Craig’s emphasis on the call, sellability/uniqueness vs frontier models, discovery interview signals (exec summary), and fit for thin slice + demo.

| Pri | Capability | One-line description | Why this rank |
|:---:|------------|----------------------|---------------|
| **P0** | **43-101–anchored project record** | Stable project/deposit identity over time: reports, issuers, renames, date semantics, facts with source/page provenance. | “43101 is the spine”; connecting dots ChatGPT doesn’t (entity resolution, history). |
| **P0** | **Multi-source public linkage** | On that spine: company, press releases, market context, QP/firm attribution from public docs—the “sources nobody’s put together” bundle. | Core platform definition on the call; tests SEDAR+, parsing, IDs. |
| **P0** | **Structured extraction** | Normalize study type, resources/reserves, economics, engineering—not geology-only. | 13A; JV/Don: geology alone isn’t enough. |
| **P1** | **Report quality & gap analysis** | Weak 43101? Missing vs Form F1 / stage peers; inconsistencies; unsupported claims—with citations. | Craig: validating poor reports is **sellable**; QA wedge (0E, 6G1, AMC). |
| **P1** | **Peer comparison** | Side-by-side normalized fields and section completeness (2–3 projects, same stage/type). | Discovery + natural second screen after extraction. |
| **P1** | **Investor / diligence brief** | Evidence-linked summary: stage, economics, open questions, comparables—trust engine, not buy/sell advice. | Investor/banker thread; Don/JV evaluator interest. |
| **P2** | **Progression over time** | Same project across successive 43101s: what changed, what’s unresolved. | 13A; JK/Don; needs 2+ reports per deposit. |
| **P2** | **Project maturity / path position** | Simplified progression model (GiM-inspired buckets): “how far along vs trajectory,” with caveats. | Layer 2; “better than nothing”; conference/BC story. |
| **P2** | **“What’s next” for explorers** | From stage + gaps + peers: **classes of work** typical before next milestone. | Craig: juniors need “what to do next to get to the next level.” |
| **P3** | **Consultant / author assist (read-side)** | Principal QA on completeness, consistency, peer norms—not full auto-draft in v0. | SRK/template workflow; avoids MNPI/drafting. |
| **P3** | **Expert-in-the-loop corrections** | Reviewer fixes record; fix persists and flows to briefs/gaps. | Layer 4; claimed moat. |
| **P4** | **First-principles geology overlay** | Deposit-type + belt context reasoning on public record. | High value, not first slice. |
| **P4** | **Permitting / ESG / social (from reports)** | Surface what’s already in 43101s (Dave’s First Nations/permitting interest)—read-only. | Good **Dave alpha** demo. |
| **Defer** | **Public QP/geologist scorecards** | FICO-like ideas on call—internal only or off v0. | Liability / 13A guardrails. |
| **Defer** | **Pre-submission drafts, corporate memory, MNPI uploads** | Per working brief. | Out of thin slice. |

### Suggested build sequence

1. **P0** (record + linkage + extraction on sample set + 1–2 BC histories if needed).  
2. **P1** — pick **either** peer compare **or** diligence brief first (whichever demo Craig leads with).  
3. **One P2** — longitudinal **or** maturity path, not both at full depth initially.  
4. **P3** — single expert-correction moment wired to one view.

### Mapping to working brief “platform” bullets

| Working brief bullet | Priority here |
|---------------------|---------------|
| Report ingestion & structured extraction | P0 |
| Evidence-linked project record | P0 |
| Technical review & gap-finding | P1 |
| Peer benchmarking | P1 |
| Progression over time | P2 |
| Maturity without a score | P2 |
| Diligence & screening brief | P1 |
| Historical reassessment | P2 (subset of progression) |
| Expert corrections that stick | P3 |

---

## (b) Demo narratives — high-level scripts

Format: **audience → hook → flow → capabilities → kill moment.**

---

### Demo 1 — “Better than ChatGPT on one BC project”

**Audience:** Craig + technical discovery contact (evaluator persona).  
**Hook:** Same question to a frontier model vs Geo.ai on one deposit with messy corporate history.

**Flow:**
1. Open hero project (Craig to pick: Red Chris, Blackwater, Galore Creek, or similar).  
2. Timeline of 43101s and key disclosures.  
3. Ask: “What changed in resource/economic story between report A and B?”  
4. Show linked answers with page citations; show issuer/name resolution.  
5. Optional: stock context at report dates (if in slice).  
6. Contrast with generic LLM answer (unlinked, wrong entity, missing reports).

**Capabilities:** P0 record, linkage, extraction; P2 longitudinal.  
**Kill moment:** Click from a number to the PDF page.

---

### Demo 2 — “Trust engine for an investor”

**Audience:** Streamer/royalty evaluator, corp dev, banker-friendly contact (not “buy this stock”).  
**Hook:** “Before partner time— is this disclosure thin or credible?”

**Flow:**
1. Two PEAs or studies from sample set (e.g. Hammerdown vs Queensway).  
2. **Diligence brief:** stage, economics, confidence flags, questions for management.  
3. **Peer panel:** same-stage peers—present vs absent (metallurgy, infra, permitting mentions).  
4. Every claim → source.  
5. Close with **questions for the company**, not a score or investment advice.

**Capabilities:** P1 extraction, gaps, peer compare, diligence brief.  
**Kill moment:** “I would ask the issuer about X before NDA.”

---

### Demo 3 — “That report’s shit—here’s why”

**Audience:** Consultancy QA (AMC/NB persona) or Craig as pseudo-SME.  
**Hook:** Expert glance: “that one’s shit; here’s why.”

**Flow:**
1. One report from training set (weak or typical).  
2. Section map vs Form F1 / stage expectations.  
3. Gap list: missing peer-common elements, inconsistencies.  
4. Side-by-side with one stronger peer at same study type.  
5. Exportable checklist for principal → junior author.

**Capabilities:** P1 gap analysis, peer compare, P3 consultant assist (read-side).  
**Kill moment:** A gap they already know, surfaced faster with documentation.

---

### Demo 4 — “Where is this project on the path?”

**Audience:** Investor, banker, conference audience (BC Roundup thread).  
**Hook:** Structured reading of distance along a development path—not “will it mine.”

**Flow:**
1. One BC deposit with history.  
2. Simplified progression model (~10–15 buckets, GiM-inspired).  
3. Place current disclosure on path with evidence (study type, resources vs reserves, known gaps).  
4. “Similar projects in this belt often still needed…” (careful, non-prescriptive wording).  
5. Clear disclaimer: not feasibility, not prediction.

**Capabilities:** P2 maturity framework, progression, P0 record.  
**Kill moment:** Non-geologist in room says the path is legible.

---

### Demo 5 — “What should we do next?”

**Audience:** Junior mining CEO / exploration VP.  
**Hook:** What work is still missing for the **next** credible disclosure milestone?

**Flow:**
1. Early MRE or PEA from sample set.  
2. Gaps vs stage-appropriate peer set.  
3. Prioritized work-program **hints** from gaps (drilling, metallurgy, env baseline)—no invented numbers.  
4. Link items to peer precedent or F1 expectations.  
5. “Take this to your QP.”

**Capabilities:** P1 gaps, P2 “what’s next,” peer compare.  
**Kill moment:** They want to screenshot the gap list for a board deck.

---

### Demo 6 — “Second discovery round in one sitting”

**Audience:** Original ~10–15 discovery network (**meta-purpose of prototype**).  
**Hook:** “You gave us round one; we built a cobbled platform—tell us what’s wrong.”

**Flow:**
1. 90-second platform map: spine + three entry views (investor, consultant, explorer).  
2. Let them pick a project they know.  
3. Run one path (brief, gaps, or timeline) by role.  
4. Ask: use on next deal/report? pay? missing?  
5. Craig captures positioning (subscription vs project eval vs public-good BC product).

**Capabilities:** Whatever is built in P0–P2; emphasis on polish and click-through.  
**Kill moment:** “Can I try another project?” not just “interesting.”

---

### Demo 7 — “Human corrects the machine once”

**Audience:** Dave (alpha) or associate geologists (later).  
**Hook:** Moat is accumulated expert correction, not the base model.

**Flow:**
1. Show a wrong or debatable extraction.  
2. Expert fixes; fix sticks on project record.  
3. Re-run brief/gaps; output reflects correction.  
4. Provenance: interpretation by reviewer, date.

**Capabilities:** P3 expert loop + downstream views.  
**Kill moment:** Dave agrees with the reading—or argues productively.

---

## Recommended demo build order

If only **2–3** demos in the first month:

| Order | Demo | Rationale |
|:---:|------|-----------|
| 1 | **Demo 2** — Trust engine / diligence | Craig’s investor/banker narrative; Roundup-ready. |
| 2 | **Demo 3** — QA / “that report’s shit” | Explicitly **sellable** on the call. |
| 3 | **Demo 1** *or* **Demo 4** | **Demo 1** if entity/history feasibility is the risk; **Demo 4** if conference abstract is the forcing function. |

**Demo 6** wraps the actual validation sessions; not a separate product surface.

---

## Open questions for Craig (and Dave when alpha)

1. **Hero deposit** for conference/abstract and Demo 1/4?  
2. Same build with **role-specific entry points**, or one linear demo for everyone?  
3. **QP/FICO language:** off marketing entirely, or internal consultant view only?  
4. **Dave alpha first:** Demo 7 (corrections) vs Demo 4 ESG/permitting slice?  
5. Confirm **data source list** in 13A §5 against thin-slice scope (working session).

---

## Pointer

- Private call transcript: `scratchpad/banks-scott-oct-16.md`  
- Analysis & feasibility backlog: `exec-summary-v1.md`  
- Proposal, guardrails, offer: `geo-ai-working-brief-v0.1.md` (Proposed path forward)
