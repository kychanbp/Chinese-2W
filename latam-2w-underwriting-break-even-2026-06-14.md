---
type: report
topic: "Should a commission-only moto-loan correspondente run its own underwriting? (break-even with grounded BR data costs)"
date: "2026-06-14"
method: "6-agent workflow: ground real BR credit-data/anti-fraud costs -> model 4 underwriting-depth strategies (free-ride / rules / fraud+FPD / full-bureau) -> 2 adversarial checks -> synthesis"
confidence: "medium-high on structure and cost anchors; exact B2B bureau pricing is contract-gated"
related:
  - "[[latam-2w-phase0-commission-read-2026-06-10]]"
  - "[[latam-2w-aggregator-pnl-2026-06-10]]"
  - "[[latam-2w-leadgen-markets]]"
---

# Should a Commission-Only Moto-Loan Correspondente Run Its Own Underwriting?

## 1. Direct verdict

**Yes — but go shallow on the data pull and deep on the engine. Run your own underwriting; do not run your own bureau.**

The naive framing ("the FI underwrites, so free-ride") and the maximalist framing ("the risk engine is the moat, so underwrite everything") are both wrong because they conflate two different things:

| | **The PULL** (data acquisition) | **The ENGINE** (model + decision logic) |
|---|---|---|
| Marginal cost | High, per-applicant, **multiplied by the funnel (×3–8)** | ~Zero once built; **falls** per-applicant as volume rises |
| Who already pays | **The FI does**, and holds the risk | **No one does it for you** |
| Duplicating it is | Value-destroying (38–66% commission haircut) | Impossible — it *is* the asset |

The correct answer: **free-ride on the FI for the expensive full bureau pull and the binding credit decision; own a single cheap score-bearing prequal that does double duty (routing + FPD/fraud screen), and run a maximally deep engine on top of that cheap data.** Depth ≠ data spend. You can run a world-class risk engine on R$4–8 of data per applicant.

---

## 2. Recommended depth: a hybrid (kill S1, kill S3) — the break-even numbers

Four candidate strategies, costed per applicant then multiplied by the funnel to get **cost per funded loan** (you pay screening on *every* applicant, earn commission on *only* funded ones — this multiplier is the whole game):

$$\text{Cost per funded loan} = \text{Cost per applicant} \times (\text{applicants per funded loan, } 3\text{–}8)$$

| Strategy | What it pulls / applicant | Cost/app (data + R$4 ops) | Cost/funded @5:1 | % of R$184 comm. |
|---|---|---|---|---|
| **S0** Free-ride | nothing | ~R$4 (intake ops only) | R$20 | 11% |
| **S1** Rules-only "routing", no bureau | CPF validation R$0.29 | ~R$4.3 | R$22 | 12% |
| **S2** Score-bearing prequal (routing + FPD) + gated biometrics | CPF R$0.29 + device/OCR R$0.16 + **score-only R$2–5** + face-match R$1–4 on riskiest ~20% (blended R$0.50) | ~R$6.5 | R$33 | 18% |
| **S3** Full CONCENTRE bureau on everyone | CPF + full report R$12–34 | ~R$24 | R$122 | **66%** |

**S3 is eliminated.** At the central 5:1 funnel it burns 38–66% of commission; at the worst 8:1 funnel its ~R$194 cost *exceeds* the R$184 commission outright. It duplicates the exact pull the FI already pays for and holds the risk on. Break-even for S3 would require a funding rate above ~75% (almost no wasted pulls) — moto funnels run 3–8:1, so **S3 never pays.** (Caveat: if the FI reimburses/shares the consulta cost, R$122 is an upper bound — but it still loses.)

**S1 is also eliminated — it's a phantom.** S1's whole premise is "route without a bureau," but **you cannot rank N lenders by expected approval without a score.** This is the hidden reason real aggregators *do* pull at prequal: FinanZero returns "up to 10 pre-approved offers in 5 minutes," which is impossible without a score-bearing pull. S1 therefore pays ops + CPF cost while delivering almost none of the routing benefit it's credited with. Delete it.

**The real fork is S2 vs S0**, and S2 wins — but the reason matters, because on *expected-value clawback alone, S0 actually beats S2:*

- Clean relative accounting: S0 net = R$184 (baseline, but fully exposed). S2 net = 184 − 33 (cost) + 6.6 (clawback avoided) + 15 (routing/table) = **~R$173.** On EV clawback alone S2 *loses* by ~R$11. The original model hid this by penalizing S0 on an absolute basis (−R$11) while crediting S2 on a relative basis (+R$6.6) — inconsistent accounting.

So S2's case does **not** rest on expected clawback. It rests on three things the EV table understates:

1. **Routing requires the score S2 buys anyway — one pull, two benefits.** The R$2–5 score-only pull simultaneously ranks lenders *and* flags FPD. Break-even on routing: a funding-rate lift of **≥~12% relative (+2.4pp absolute, e.g. 20%→22.4%)** recovers S2's full cost. Achievable in a multi-lender panel. And a single **+0.3pp table improvement** (1.7%→2.0% on a R$12k ticket) = **+R$36/funded**, which alone dwarfs S2's entire R$33 cost.
2. **Fraud carries "100% commission + liability," not just commission.** The givens specify indemnity exposure beyond the reversed commission. The avoided loss per caught fraud is *commission + liability* (potentially multiples of R$184), so the fraud gate is justified at a **lower** bad-rate threshold than the R$184-capped EV math implies. This is tail-risk insurance, not EV.
3. **Gating, not blanket.** Blanket biometrics on 100% of applicants needs a ~16% combined FPD+fraud rate to pay. Risk-gated to the worst ~20%, break-even drops to **~3%** combined FPD+fraud — which moto/autônomo segments routinely exceed. So gate, never blanket.

**Recommended strategy: S2-hybrid** — one cheap score-bearing prequal pull per applicant (routing + FPD), plus a risk-gated identity/biometric check on the high-risk slice only. Net ≈ R$173–183/funded vs S0's R$173-but-exposed and S3's R$88.

---

## 3. Data-spend tiering rule

The discriminating test is **not "is it cheap"** — it's **"who owns the resulting signal."**

> **Free-ride on the FI for any signal whose value is fully captured by the FI's own risk decision. Own — and go arbitrarily deep on — any signal whose value accrues to *you* (clawback) or is *not in the FI's possession* (thin-file moto lift, routing, cash-flow).**

| Tier | Signal | Spend ceiling | Why |
|---|---|---|---|
| **Tier 0 — Free-ride** | Full bureau report (CONCENTRE, R$12–34); the binding credit decision; the balance sheet | **R$0 — never buy** | FI already pays and holds the risk. Duplicating = 38–66% haircut for zero marginal protection. |
| **Tier 1 — Cheap, always** | CPF/situação cadastral (R$0.20–0.51); device fingerprint/OCR (R$0.16); **score-only / restritivos (R$2–5)** | **Hard ceiling ~R$4–8/applicant** | The funnel multiplier (×3–8) means per-applicant pull is the one thing that *must* stay cheap. The score does double duty: route + FPD. |
| **Tier 2 — Risk-gated** | Face-match / liveness (Unico/idwall/ClearSale, R$1–4); deeper alt-data | **Only on riskiest ~20%** (blended ~R$0.50/app) | Blanket needs 16% bad rate to pay; gated needs only ~3%. Pull conditionally, triggered by Tier-1 flags. |
| **Tier 3 — Consented conversion step** | Open Finance cash-flow / PIX | **~R$0 rail** | The thin-file moto edge. Not a silent pull — a conversion UX step. This is where you out-underwrite the bureau. |

Pull-order discipline also minimizes the *consulta-clustering* score damage: in Brazil the customer's own score check is harmless, but multiple *company* credit consultas in a short window signal "busca intensa por crédito" (~12% of score weight). Routing to the single best-fit lender *first* — instead of fanning the CPF to all N lenders — protects the customer's score and lifts downstream approval. That's the real routing mechanism.

---

## 4. Where underwriting flips from cost to moat/revenue

Inside the current deal (commission-only, FI holds risk), underwriting is a cost center — which is why the data pull must stay shallow. **The moat lives in the engine, and its payoff shows up in the *next* contract, not this quarter's commission line.** All three payoffs require the engine to be **demonstrably accretive over the FI's own screen** — a higher bar than "cheap enough not to lose money."

| Flip point | Mechanism | What it requires |
|---|---|---|
| **Better tables (ratchet)** | A proven low-FPD book is *evidence* you bring to the FI to renegotiate the upfront % upward over time. +0.3pp = +R$36/funded; repeated, it compounds. | A logged FPD track record showing your screen is accretive. |
| **FLDG / spread participation (the regime change)** | Move from commission-only to **risk-sharing** (FLDG, partial spread, co-lending) — a categorically larger, more durable P&L than a 1.7–3% commission. You cannot ask for FLDG terms without an engine that *proves your screen adds predictive power over the FI's.* | Engine demonstrably accretive on the segment. **The engine is the entry ticket to a different P&L.** |
| **Screening-as-a-service** | Once the engine is good, your calibrated fraud/FPD score on the thin-file moto-autônomo segment (which bureaus serve poorly) becomes **sellable to other FIs and correspondentes.** Increasing returns: more volume → better model → more saleable → more volume. The routing log *is* the training set. | Proprietary data exhaust + proven lift. |

**Sequencing:** (1) *Now* — shallow pull, deep fraud/FPD + routing engine, accumulating a proprietary accretive track record on the thin-file segment; you underwrite not to *decide* (the FI decides) but to *prove and to protect your clawback.* (2) *Next* — present "my screen drops FPD by X over your panel" to renegotiate tables, then claim an FLDG seat. (3) *Later* — sell the screen; consider principal/co-lending only if it justifies leaving capital-light. The founder's antifraud/credit-risk edge + R$4/app AI-ops is exactly the team to build the deepest engine on the cheapest data.

---

## 5. The single number to track

**Incremental FPD lift of your screen over the FI's own screen — i.e., the percentage-point reduction in first-payment-default (and fraud) rate on the loans *you* pre-approved versus a no-own-screen baseline, on the moto/autônomo segment.**

$$\Delta\text{FPD} = \text{FPD}_{\text{FI screen alone}} - \text{FPD}_{\text{FI screen} + \text{your screen}}$$

Why this one number governs everything:

- **It is the break-even gate today.** Every point of FPD/fraud you remove is up to 100% of commission (+ liability) saved on a clawback you'd otherwise eat blind. Your screen pays for itself the moment ΔFPD × (commission + liability) per funded loan exceeds your screening cost (~R$33/funded for S2-hybrid). At commission R$184 and gated cost R$33, you need to avoid roughly **one clawback per ~6 funded loans of marginal effect** — a low bar on thin-file moto.
- **It is the moat metric tomorrow.** ΔFPD > 0 and durable is the *exact* evidence that converts a commission into better tables, then into an FLDG/spread seat, then into a sellable score. If ΔFPD ≈ 0, your screen is not accretive — you're paying the rent but building no moat, and you should fall back toward free-riding.

Track ΔFPD per cohort, per segment, per lender. It is simultaneously the answer to "is my underwriting paying *this quarter*?" and "is my underwriting becoming the *moat*?" — which is precisely why it's the one number to watch.

---

*Sources (inline): commission/funnel/clawback figures and R$4/app ops target — vault corpus (given). Brazilian cost anchors — CPF/situação cadastral R$0.20–0.51 (Receita/BigDataCorp); device/OCR R$0.16 (BigDataCorp); Serasa Score e Atributos API R$2–5 (serasaexperian.com.br/solucoes/score-e-atributos-api); full third-party report ~R$35 retail / R$12–34 B2B (serasa.com.br/consultar-meu-cpf); face-match/liveness R$1–4 (Unico/idwall/ClearSale, quote-gated). Routing/free-ride structure — correspondente submits proposal, FI makes binding decision (vivareal.com.br); FinanZero multi-lender routing, "up to 10 pre-approved offers in 5 min," lead-commission model (exame.com). Soft-pull mechanic — company credit consultas register and signal "busca intensa por crédito" (~12% score weight); consumer's own check is harmless (serasa.com.br/score/blog).*