# The AI Pilot-to-Product Playbook
### A lightweight governance operating model for small-to-medium enterprises

**Version:** 0.9 (Draft)
**Owner:** [Executive Sponsor — CEO / COO / CIO]
**Cadence:** Monthly AI Investment Council; quarterly portfolio review
**Scope:** All AI initiatives — pilots, proofs-of-concept, vendor trials, embedded AI features — regardless of budget size

---

## 1. The problem this playbook solves

Most SMEs don't lack AI pilots. They lack a way to decide **which pilots deserve to become products.**

The typical failure pattern:

1. Someone demos a tool; enthusiasm spikes.
2. A pilot launches with no defined success criteria.
3. Three months later, nobody can say whether it worked.
4. It quietly dies — or worse, it quietly lives on, consuming licenses and attention.
5. Repeat, five times over. Now there are seven pilots, no shared risk posture, and no realized value on the P&L.

The root cause is not a lack of innovation or budget. It's the absence of a **decision loop** — one repeatable path from idea → investment → evidence → scale-or-stop.

This playbook installs that loop with three components:

| Component | What it does | Artifact |
|---|---|---|
| **Use-case intake** | Every idea enters through one door, scored the same way | One-page intake brief |
| **Risk review** | Right-sized, proportionate to exposure — not a legal gauntlet | Risk screen + tiered review |
| **Value tracking** | Every funded pilot carries a value hypothesis measured against reality | Value ledger + exec dashboard |

Bound together by a **three-gate funding model** with explicit decision rights, so the question at every stage is never "is this interesting?" but **"should this get the next dollar?"**

**Design principles:**

- **Proportionate, not bureaucratic.** A $5K pilot and a $250K platform build should not face the same paperwork — but both should face the same questions.
- **Kill fast, scale deliberately.** The most valuable governance decision is a fast, blameless "stop."
- **Realized value is the only scoreboard.** Projected value gets you funded; realized value gets you scaled.
- **One owner per initiative.** A business owner, not IT, accountable for the value hypothesis.
- **Time-to-decision is a first-class metric.** If governance takes longer than the pilot, the pilot will route around it.

---

## 2. Operating model at a glance

```
        ┌─────────────────────────────────────────────────────┐
        │              AI INVESTMENT COUNCIL (monthly)         │
        │   CFO · Business lead · Tech lead · Risk/legal · HR  │
        └───────┬──────────────────┬──────────────────┬────────┘
                │                  │                  │
        GATE 0 ▼          GATE 1 ▼          GATE 2 ▼        GATE 3 ▼
        ┌───────┐  ~30d   ┌───────┐  ~60d    ┌───────┐ ~90d   ┌───────┐
  Idea →│ INTAKE│────────▶│ PILOT │─────────▶│PROVE  │───────▶│ SCALE │──▶ Product / BAU
        │ +SCORE│         │ $ ≤X  │          │$ ≤Y   │        │ $ ≤Z  │
        └───────┘         └───────┘          └───────┘        └───────┘
             ▲                  │                 │                │
             │                  └── Stop ◀────────┘ ◀──────────────┘
             │                        (blameless kill, documented lesson)
             └─────── portfolio review re-ranks everything quarterly ──┘
```

**Roles (keep this to five, max):**

| Role | Who (SME-sized) | Accountable for |
|---|---|---|
| **Executive Sponsor** | CEO, COO, or CIO | Removing blockers; final escalation |
| **AI Investment Council** | CFO + business owner + tech lead + risk/legal + HR (one meeting/mo) | Gate decisions; portfolio ranking |
| **Initiative Owner** | A named business-line manager | The value hypothesis, adoption, and results |
| **Technical Lead** | IT / head of engineering | Feasibility, security, integration, vendor posture |
| **Risk Partner** | In-house counsel, fractional GC, or retained advisor | Risk tiering, policy sign-off, compliance |

> In a 50-person company, one person may hold two of these roles. What matters is that **every initiative has a named Initiative Owner who is not in IT** unless the value accrues to IT itself.

---

## 3. Stage 1 — Use-case intake

Every AI idea — internal, vendor-pitched, or executive whim — enters through a **one-page intake brief**. If it can't be filled out in 30 minutes, it isn't ready to be a pilot.

### 3.1 The one-page intake brief

```
INITIATIVE:   ______________________     DATE: __________
OWNER:        ______________________     (business, not IT)

1. PROBLEM      What pain, cost, or opportunity does this address?
                Who feels it today, and how much does it cost/delay?

2. THE AI BET   In one sentence: what will AI do that couldn't be done
                (or wasn't affordable) before?

3. USER         Who uses it, how often, and what do they stop doing?

4. VALUE HYPOTHESIS (pre-registration)
   ┌ We believe this will [reduce cost / grow revenue / reduce risk]
   ┌ by [X% or $X] for [scope], measured by [metric], within [N months].
   ┌ Baseline today: ______ (attach how it was measured)

5. SMALLEST     What is the cheapest version that produces real evidence?
   HONEST TEST  What would we need to see to say it failed?

6. FEASIBILITY  Data available? System integration? Skills on hand?
                Build / buy / configure?

7. RISK SKETCH  Customer data? Automated decisions on people?
                Regulated domain? Vendor stability? (Section 4 tiers this)

8. ASK          Gate 0 budget: $______   Duration: ____ weeks
                People-days committed: ______
```

**Intake rules:**

- **No brief, no meeting.** The Council doesn't hear verbal pitches; it reads one-pagers. This alone cuts pilot sprawl dramatically.
- **The value hypothesis must be falsifiable.** "Improve efficiency" is not a hypothesis. "Cut invoice-processing time from 11 min to 6 min for AP's 3-person team, verified by system logs, within 8 weeks" is.
- **Baseline first, always.** A pilot without a measured baseline cannot prove value later. If you can't measure the baseline, that's a Gate 0 finding, not a pilot detail.
- **Cap concurrent pilots** at roughly **one per 25 employees** (e.g., max 4 in a 100-person firm). The constraint is attention, not money.

### 3.2 Scoring: value, feasibility, risk

Each intake is scored on three axes by the Council in ~10 minutes. Score 1–5 each; the combination drives both funding priority and review depth.

**Value (revenue, cost, risk-reduction):**

| Score | Signal |
|---|---|
| 5 | Directly moves revenue or cuts ≥$250K/yr at full adoption |
| 3 | Cuts $25K–250K/yr, or frees meaningful capacity |
| 1 | "Everyone says it would be cool" — no costed baseline |

**Feasibility (data, integration, skills, vendor):**

| Score | Signal |
|---|---|
| 5 | Data ready, off-the-shelf, one integration, skills on staff |
| 3 | One real dependency (e.g., data cleanup, new vendor contract) |
| 1 | Needs data we don't collect, custom build, or key-person dependence |

**Risk (downside if it fails or misbehaves):**

| Score | Signal |
|---|---|
| 5 | Internal, low-stakes, human-in-the-loop, easily reversible |
| 3 | Touches customer data or influences decisions on employees/customers with human review |
| 1 | Automated consequential decisions, regulated domain, or unvetted vendor |

### 3.3 Portfolio map: where initiatives land

Plot every in-flight initiative on the two views below. **Update quarterly; review the map at every Council meeting.** The map is the single artifact executives should look at to answer "are we working on the right things?"

**View A — Value × Feasibility** (bubble size = ask $; risk shown as border)

```
 FEASIBILITY
   ▲
 5 │  ┌─────────────┐
   │  │  DO NOW     │              ┌─────────────┐
 4 │  │ fund fast,  │              │  PLAN/DE-RISK│
   │  │ prove in 60d│              │ fix data or  │
 3 │  └────┬────────┘              │ vendor first │
   │       │ high-value             └──────┬──────┘
 2 │       │ high-friction          low-value,
   │       │ = classic              high-friction
 1 │       │ quick-win zone          = KILL (or park)
   └───────┼──────────────────────────────▶ VALUE
          low                            high
```

- **High value, high feasibility →** fund at Gate 1 immediately.
- **High value, low feasibility →** fund a *de-risking* step (data cleanup, vendor diligence), not the pilot itself.
- **Low value, high feasibility →** acceptable only as a cheap capability-builder (learning pilot with a hard $ cap).
- **Low value, low feasibility →** kill. Politely, immediately, with a thank-you.

**View B — Risk × Value** (determines review depth, not just priority)

```
              RISK ▲
                   │  [Tier 3: CONFINED]      [Tier 2: GUARDED]
                   │   full Council review,    Council + risk partner
                   │   legal sign-off before   sign-off; human-in-loop
                   │   any customer exposure   mandatory
                   │
                   │  [Tier 4: PARKED]         [Tier 1: OPEN]
                   │   automated consequential  self-serve; Council
                   │   decisions in regulated   informed, not gated
                   │   domains — don't proceed
                   │   until controls exist
                   └────────────────────────────▶ VALUE
```

### 3.4 Risk tiers (proportionate review — the anti-bureaucracy mechanism)

| Tier | Definition | Examples | Review required |
|---|---|---|---|
| **1 — Open** | Internal tools, no personal data beyond employee use, human does the final call | Draft-generation assistant, internal search over docs | Council informed; standard IT security check |
| **2 — Guarded** | Customer or employee personal data; outputs influence decisions with human review | Support-ticket triage, resume screening *with* human decision, churn scoring | Risk partner sign-off; documented human-in-the-loop; vendor DPA |
| **3 — Confined** | Automated or semi-automated decisions affecting individuals; regulated data (health, finance); external-facing output at scale | Automated credit/pricing decisions, AI-generated customer comms unsupervised | Full Council review + legal; escalation path; disclosure plan; audit log |
| **4 — Parked** | Consequential automated decisions in heavily regulated domains without adequate controls | Fully automated hiring rejection, medical advice delivery | Do not proceed. Revisit when controls exist. |

**Rule of thumb:** *the tier sets the review depth, never the ambition.* A Tier 3 idea isn't banned — it's sequenced: prove it as a Tier 2 human-in-the-loop pilot first, then earn automation.

**Minimum risk controls for Tier 2+:** vendor data-processing agreement · no training on our data without explicit terms · named human accountable for outputs · simple override/rollback · 15-minute written risk note (what could go wrong, who's harmed, what's the control). Do **not** build a model-risk committee. You don't need one; you need someone to ask the questions out loud.

---

## 4. The three-gate funding model

Money is released in tranches. Each gate asks one question and has one decision owner. Gates are **calendar-boxed** — a pilot that can't hit its gate in the allotted window has already answered the question.

| Gate | Name | Question | Typical funding | Duration | Decision owner |
|---|---|---|---|---|---|
| **0** | Intake & Triage | Is the problem real and is the smallest honest test defined? | $0–10K (setup only) | — | Council (consent; 15 min/item) |
| **1** | Pilot | Does it work in our environment, with our users, at honest fidelity? | ≤ $25K / ≤ 90 days | 30–60 days | Council |
| **2** | Prove | Does it measurably deliver the value hypothesis at production fidelity? | ≤ $75K cumulative | 60–90 days | Sponsor + CFO |
| **3** | Scale | Is it a product? Who owns it in BAU, at what run-rate? | Business case | 90+ days | Sponsor (CFO countersigns run-rate) |

> Calibrate the dollar bands to your company: the intent is that **no single unproven idea can consume more than ~1% of revenue** before reaching Gate 3.

### Gate 0 — Intake & Triage *(Council, 15 minutes per item)*

**Decision:** Fund a Gate 1 pilot / De-risk first / Decline / Park (Tier 4).

- Score on value/feasibility/risk; assign risk tier; assign Initiative Owner.
- **Kill criteria set at entry:** the Council and Owner agree in advance what "failed" looks like. This is the single highest-leverage governance act in the whole playbook.
- **SLA: decision within 10 business days** of intake. Time-to-decision here is a tracked metric (§6).

### Gate 1 → 2 — Pilot to Prove *(Council)*

The pilot's job is to produce **evidence, not enthusiasm.** To pass:

| Evidence | Standard |
|---|---|
| Value signal | ≥ 50% of the projected per-unit improvement (e.g., projected 11→6 min; pilot must hit ≤ 8.5 min) |
| Adoption | ≥ 60% of the pilot user group used it ≥ 2×/week without being chased |
| Reliability | Output accepted/used ≥ 80% of the time (human overrides are counted, not hidden) |
| Risk | Operating within declared tier; zero unmitigated Tier 2+ findings |
| Unit economics | Cost per unit of work plausible at 10× volume |

**Decisions:** Advance to Gate 2 / Extend once (max 30 days, pre-stated reason) / **Stop** / Pivot (re-enters intake with lessons — a pivot is a new one-pager, not a continuation).

### Gate 2 → 3 — Prove to Scale *(Sponsor + CFO)*

The pilot becomes a small production deployment with real users and real measurement. To pass:

- **Realized value ≥ 70% of projection** over the Gate 2 window, measured by the same method as the baseline.
- **Adoption sustained** (not just launch-week curiosity): usage stable or growing over 8+ weeks.
- **Run-rate known:** licenses, hosting, support, retraining, model/API cost at scale — itemized.
- **Operational owner named** in the business line, with IT run-book (who fixes it when it breaks at 9am Monday).
- **Risk controls survive scale:** human-in-loop design, escalation path, and audit trail still work at 10× volume.

**Decisions:** Fund as product (BAU budget, not innovation budget) / Hold at current scope (occasionally the honest answer: valuable locally, not worth scaling) / Decommission with a documented handoff.

### Gate 3 — Scale governance (ongoing, quarterly)

Scaled products aren't exempt; they enter **quarterly value reviews**: realized value vs. projection, drift/quality incidents, cost creep, and vendor risk. A product that misses realized-value targets for two consecutive quarters triggers a fix-or-sunset decision. AI products depreciate faster than software — sunset criteria are set at scale time, not improvised later.

### Decision rights summary (RACI, compressed)

| Decision | Owner | Consulted | Informed |
|---|---|---|---|
| Idea accepted / declined (Gate 0) | Council | Risk partner | All staff via monthly note |
| Pilot funding ≤ $25K | Council | Tech lead | Sponsor |
| Stop a pilot | Council (Owner may self-stop anytime) | — | Sponsor |
| Scale funding (Gate 3) | **Sponsor** | CFO, Risk | Council |
| Risk tier assignment | Risk partner | Tech lead | Council |
| Kill criteria at entry | Initiative Owner proposes; Council approves | — | — |
| Vendor selection (data terms) | Tech lead + Risk partner | Owner | Council |

**Escalation:** any gate decision may be escalated to the Sponsor once, with a written one-paragraph case; Sponsor decides within 5 business days. **Silence past an SLA = the initiative advances** (governance must never be the slowest node in the system).

---

## 5. Value tracking — the value ledger

Every funded initiative gets a row in the **value ledger** — a single spreadsheet is genuinely sufficient at SME scale. Nothing else in this playbook works without it, because it is the connective tissue between intake, gates, and the dashboard.

| Field | Example |
|---|---|
| Initiative / Owner | "AP invoice copilot" / Maria (Finance) |
| Risk tier | 2 — Guarded |
| Gate / tranche to date | Gate 2 / $40K |
| Value hypothesis | Cut invoice processing 11→6 min (−45%) |
| **Baseline (measured)** | 11.2 min/invoice, 1,400 invoices/mo |
| Current measurement | 7.9 min/invoice (system logs, wk 6) |
| **Projected annual value** | $63K labor capacity + $8K late fees |
| **Realized value to date** | $21K (3 months at current delta) |
| Adoption | 78% of AP team, 4.1 uses/wk, trending flat |
| Next gate / date | Gate 3 review — Mar 15 |
| Decision due | Scale / Hold / Stop |

**Rules that keep the ledger honest:**

1. **Realized ≠ projected.** Realized value is counted only when (a) the baseline method matches the measurement method, and (b) the saving is *actually redeployed or captured* — hours freed that nobody reclaims are not dollars saved.
2. **One measurement method, end to end.** If the baseline was a stopwatch estimate and the pilot result is system-logged, you don't have a result; you have a narrative. Pick the cheaper honest method and use it both times.
3. **No self-graded homework.** The CFO (or delegate) validates any value claim used for a gate decision. Two minutes of checking prevents most value inflation.
4. **Leading indicators get logged, not celebrated.** User satisfaction and usage frequency are diagnostics; they never substitute for the value metric at a gate.
5. **Count the full cost.** Licenses + implementation time + ongoing support + the Owner's hours. A pilot that saves $30K while consuming $45K of staff time is a finding, not a failure of accounting.

---

## 6. The executive dashboard

One page. Reviewed monthly by the Council, quarterly by the leadership team. Built in whatever BI/spreadsheet tool exists — the discipline matters, not the software.

### Panel A — Portfolio funnel

| Metric | Definition | Healthy signal |
|---|---|---|
| Ideas in intake | Briefs submitted this quarter | — |
| Time-to-decision (Gate 0) | Median days from brief to Council decision | **< 10 business days** |
| Active pilots | Funded, in Gate 1–2 | ≤ 1 per 25 employees |
| Kill rate | Pilots stopped before Gate 3 | **30–50%** — *low kill rates mean you're not gating, high ones mean Gate 0 is rubber-stamping* |
| Time-to-decision (all gates) | Median days at each gate vs. SLA | ≥ 90% within SLA |
| Pilots stalled > 60 days | No gate movement | 0 — each gets a fix-or-stop call |

### Panel B — Value realized vs. projected

| Metric | Definition |
|---|---|
| Projected portfolio value | Sum of annualized value hypotheses for active initiatives |
| **Realized value (validated)** | CFO-confirmed savings/revenue, trailing 12 months |
| **Realization ratio** | Realized ÷ projected — the health metric of the entire governance loop (target ≥ 60% for things that pass Gate 2; if it's 15%, projections are fiction — tighten Gate 0) |
| Value by function | Where value is landing (ops, finance, sales, support) — exposes concentration risk |
| Total cost of AI portfolio | Licenses + build + support + staff time |

### Panel C — Adoption & operations

| Metric | Definition | Healthy signal |
|---|---|---|
| Active usage | % of intended users active weekly | > 60% post-Gate 1 |
| Habit depth | Median uses per active user per week | ≥ 2 |
| Adoption trend | 8-week slope | Flat-or-up; a decayed pilot is a stopped pilot |
| Overrides / corrections | Rate humans reject AI output | Falling over time; spikes trigger review |
| Incidents | Quality/privacy/security events, by tier | Zero unmitigated Tier 2+ |
| % spend on Tier 2/3 systems | Concentration of governed risk | Tracked, no target — visibility is the point |

**Dashboard presentation:** a traffic-light portfolio map (§3.3) on the left; the five headline numbers — *median time-to-decision, realized vs. projected value, realization ratio, portfolio adoption, active pilot count* — across the top. If the leadership meeting spends its time on anything else, the dashboard is too complicated.

### What "good" looks like after 12 months

- Median idea-to-decision under 10 days; every pilot had kill criteria at entry.
- A kill rate in the 30–50% band — and **no stigma attached to it.** The Council's best decision of the year should be a fast stop that freed $40K and two people.
- Realization ratio ≥ 60% on scaled items, with a CFO-validated trail.
- 1–3 AI products in BAU with named operational owners and known run-rates.
- Zero governance meetings longer than 60 minutes.

---

## 7. First 90 days — implementation plan

| Weeks | Action | Output |
|---|---|---|
| 1–2 | Sponsor names the Council (5 people); adopt this doc as v1.0 | Charter signed; monthly 60-min meeting booked |
| 2–3 | Inventory every in-flight AI pilot; force-rank with value/feasibility/risk scores | Portfolio map v1 — expect 30–50% to be immediately killable; that's a feature |
| 3–4 | Build the value ledger; measure baselines for the 3–5 survivors | Ledger live; every survivor has an Owner and kill criteria |
| 5–6 | First Council meeting: run gates on the ranked list; publish decision SLAs | First decisions made *and published* — visible decisions are the product |
| 6–12 | Run the loop; publish the dashboard monthly; hold the first quarterly portfolio review | Dashboard v1; first stop decisions made blamelessly |
| 13 | Retro: what did the loop make slower that wasn't worth it? What risk did it miss? | Playbook v1.1 |

**Common early traps:** recreating a corporate PMO (resist — five roles, one page, one spreadsheet) · letting vendors brief executives before they write an intake brief · scoring every idea Tier 1 to avoid the risk conversation · letting the innovation budget silently become an operations budget after Gate 3 · measuring adoption but never value.

---

## Appendix A — Gate 1 exit memo template *(one page max)*

```
INITIATIVE: ___________   GATE: 1→2   DATE: ______
OWNER: ___________

1. HYPOTHESIS (from intake): ...
2. RESULT vs. HYPOTHESIS: ... (same method as baseline)
3. ADOPTION: users __ / target __   frequency __ /wk   trend ↑ → ↓
4. RELIABILITY: acceptance __%   overrides __%   incidents: __
5. COST TO DATE: $____ (incl. staff days: __)
6. RISK: tier __ · changes since Gate 0: __ · open findings: __
7. RECOMMENDATION:  Advance / Extend / Stop / Pivot
   Because: ... (3 sentences max)
8. IF ADVANCE: Gate 2 budget $__, duration __ wks, measurement plan: ...
   IF STOP: what we learned (3 bullets), what gets redeployed: ...
```

## Appendix B — Council meeting agenda *(60 minutes, monthly)*

1. **Metrics on the wall** (10 min): dashboard headline numbers; any SLA misses.
2. **Gate decisions** (25 min): read memos in advance; 5 min per item; decide in the room.
3. **Portfolio map review** (10 min): new ideas scored; anything stalled > 60 days gets fix-or-stop.
4. **Risk scan** (10 min): new Tier 2/3 items; vendor changes; incidents.
5. **One improvement** (5 min): one thing to make the loop faster or sharper next month.

## Appendix C — Blameless stop protocol

A stopped pilot is a **priced, documented learning** — the cheapest failure in the portfolio. Protocol: Owner writes three lessons (≤ 15 min) → Council thanks the owner publicly → any reusable assets (prompts, data work, vendor terms) are logged → the kill is recorded on the portfolio map, not buried. **If anyone's reputation suffers for a well-run stop, the governance loop is broken** — people will hide pilots, and hidden pilots are the actual risk this playbook exists to prevent.
