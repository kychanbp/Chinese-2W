---
type: validation
topic: "Comprehensive re-evaluation — data, logic, claims & conclusions of the Brazil moto-finance aggregator research"
date: "2026-06-10"
method: "4 independent reviewers (24-figure fact-check w/ primary sources · adversarial logic audit · conclusions stress-test · information-value/gap audit)"
related:
  - "[[latam-2w-leadgen-markets]]"
  - "[[latam-2w-brazil-lender-landscape-2026-06-09]]"
  - "[[latam-2w-comparables-teardown-2026-06-07]]"
---

# Comprehensive Re-evaluation — 2026-06-10

Four independent reviewers re-audited the entire corpus (site + 10 reports + wiki): every load-bearing figure against primary sources, the logic of each claim, and whether the conclusions follow. **Headline: the market-structure spine verifies cleanly, but three load-bearing figures were wrong in the thesis-flattering direction, the verdict overstated ("validated on paper" → "structure validated; economics unmodeled"), and the Phase-1 design needed a Gate-0 + desk-sprint redesign.** All corrections applied to the site and wiki same-day.

## 1 · Fact-check (24 figures, primary-source verified)

### Wrong / misleading — fixed on the site

| # | Figure | Verdict | Correction |
|---|---|---|---|
| 1 | "~47% of Honda sales financed" | **MISLEADING** | Honda Serviços Financeiros = 47% of Honda's 2025 sales, but **~32pp consórcio + ~15pp Banco Honda CDC**. True loan penetration ~15% — the CDC pool the aggregator monetizes is ~3× smaller than the headline implied. |
| 2 | "Used motos lead financing volume (116k vs 46k)" | **WRONG — inverted** | B3/SNG Nov 2025: **116k NEW vs 46k used**. New out-finances used ~2.5:1; used is the *underserved minority* (~28% of contracts) — still Omni's white space, but the volume claim was backwards. |
| 3 | Move Motos = "R$30bn BNDES, terms pending" | **WRONG MP + STALE** | R$30bn = the **car/taxi** track (**MP 1.362/2026**; MP 1.360 is the mototáxi CTB rules). Move Motos terms now out: **~R$4bn**, ~12.6%/yr, ~R$20k/CPF, contracting from 19 Jun 2026. The EV gate is a R$4bn program, 7.5× smaller than implied. |
| 4 | Mexico "35% China tariff" | **WRONG (over-correction)** | Final DOF decree (Dec 2025, eff. Jan 2026): **motorcycles 25%**; 35% was the Sep-2025 *proposal*. |
| 5 | "China 2W exports $14.5B / 36.75M units" | **MISLEADING (mixed universes)** | $14.5B (+25.4%) = HS-8711 motorcycles ✓; **36.75M units blends e-bikes** (moto-only ≈ 11–13M). Decoupled on the page. |
| 6 | Galgo funding "$72–153M" | **WRONG range** | **~$83.8M total** equity (PitchBook); $40.8M Series B (2023). |
| 7 | Correspondente rule "Res. 3.954/11" | **STALE** | **CMN Res. 4.935/2021** (in force Feb 2022) — same mechanism + certification requirement. |

### Verified correct (the spine holds)

Brazil 2,197,308 motos 2025 (+17.1%, Fenabrave) · Honda 66.8% · Italika ~65–70% MX · moto financing +10–18% 2025 vs cars stalled (B3) · consórcio 30.8% of sales (ABAC) · PAN ~33–35% (company-claimed) · **Galgo MX/CO/CL/PE, no Brazil entity as of Jun 2026** · Omni ~3.9% a.m. negativado · Voltz RJ Nov 2023, R$335M · Meta AI agent global 3 Jun 2026 · FinanZero ~10% approval (2021 vintage, flagged).

## 2 · Logic & claims audit (adversarial) — top findings

1. **KILL-RISK — the aggregator's P&L was never modeled.** Every quantitative model in the corpus prices the *abandoned lead-gen* version (verdict: −$0.10/lead). The live model's revenue ≈ **R$180–240 (~$33–44) per funded ~R$12k loan** (1.5–2% commission); at FinanZero-like ~10% approval, cost-per-funded-buyer plausibly exceeds it. "Validated on paper" rested on a P&L that doesn't exist.
2. **KILL-RISK — "waterfall out-approves" is undercut by its own comparable.** FinanZero runs the exact mechanic with 50–60 FIs at **~10% approval** — a panel mostly re-shops the same bureau-negative buyer to lenders with overlapping policies. Consórcio "approvals" deliver no bike (until contemplated) and shouldn't count.
3. **KILL-RISK — every "gap" has an adverse-selection explanation the corpus itself derived, then dropped:** tiny tickets + same underwriting cost + worse collateral = negative ROI for incumbents with *lower* costs. MercadoLivre excluding motos and FinanZero keeping moto CDC thin despite 70+ FI partners are revealed-preference evidence the lane may be economically bad, not just open.
4. **Contradiction:** lane report says FinanZero does moto-*collateral* refi only; teardown says it markets moto-*purchase* CDC. Load-bearing for "no one does this" — if FinanZero already runs multi-FI moto-purchase CDC, the white space shrinks to UX + dealer channel (copyable in a quarter). Resolve from the live product.
5. **The single-bank-loja premise is asserted, not evidenced** — PAN runs a 20k-store lojista program; Omni's distribution *is* lojista partnerships; the dealer's cheapest counter is signing two more correspondente contracts itself. Make "ICP lojas are single-bank with material rejection piles" an R2 *measurement*.
6. **Unverified contractual question:** will a lender book purchase-money CDC where the correspondente is a *non-selling third party* at someone else's POS? (Multi-FI brokering per se is settled — Creditas is simultaneously correspondente for Santander/Itaú/Porto/Bradesco.)
7. **Affordability, not approval, may be the bottleneck:** Omni's negativado terms are ~3.9% a.m. (≈58%+/yr CET) with 20–50% down — approvals can die on the entrada. Track approved-but-can't-fund separately.
8. **"One empirical crux" was false framing** — acquisition, thin-file prequal, lender onboarding, dealer cooperation, approved→funded conversion. Masthead now matches candor.
9. **"TikTok = owned-audience moat" had zero evidence** (no CAC data anywhere in the corpus) — downgraded to unproven hypothesis; **paid traffic is already ruled out by arithmetic** (cost/funded must beat ~$40).
10. **Voltz miscast:** an EV-hardware/balance-sheet failure, not evidence "integration failed in Brazil" — meanwhile Mottu, an integrated operator, is succeeding there.

## 3 · Conclusions stress-test — verdict: SOUND-WITH-CHANGES

Direction (cheap kill-gated test, ICE-first, dealer-QR primary) follows from the evidence; the Phase-1 as written would have burned budget without a decidable answer:

- **R1 "3 lenders live by wk 3" was fantasy** — FBB-130 cert is days (~R$150), but per-bank credenciamento of a no-storefront broker is weeks–months (PAN has closed lojista intake before). Fast path: promotora/master-correspondente, or rent supply via Juros Baixos CaaS / FinanZero partnership.
- **Several "field tests" are phone calls:** commission % (CMN cap 6%; typical 1.2–1.8%), clawback terms, multi-FI permission, third-party-at-POS — all week-1 desk reads from the contracts.
- **Kill-gates had regressed to measurements.** Restored thresholds: n≥100 dealer-rejected applicants · panel approval ≥25% · approved→funded ≥50% · cost/funded < commission · ≥20 funded loans, commission cash received.
- **R2 was underpowered:** 3–5 lojas ≈ 25–40 rejects in the window → expanded to 8–12 lojas, concierge/manual waterfall (build nothing).
- **Missing Gate 0:** a named PT-BR local operator + CNPJ path — every Phase-1 task is in Portuguese on the ground. No operator → no-go regardless of economics.
- **Scale arithmetic:** the rejected-buyer wedge ≈ R$500–750/loja/mo → a ~$500k/yr business needs **150–300+ lojas** or insurance attach / whole-flow capture (the Rupyy "2W too thin alone" lesson). The 90-day test reads unit economics only, not the scaling question.
- **Honest envelope: ~120–130 days, $4–6k with a partner CNPJ ($8–15k without).**

## 4 · Information-value gaps (next analyses, ranked)

1. **Aggregator-native unit economics** (the one-day analysis that should precede any spend): contribution/funded-loan = commission% × ticket − CAC/funded − ops; breakeven volume; commission%-×-CAC frontier.
2. **Origination-revenue TAM:** ~2.2M units × ~32% financed × ~R$12k ≈ **R$8–9B/yr** Brazil moto-CDC origination; × commission% = revenue pool; SAM = challenger-ICE/thin-file/used slice (plausibly 5–15%).
3. **New competitive signal: TikTok itself applied to BACEN for IP + SCD (lending) licenses in Brazil** — the acquisition channel's owner is becoming a lender. Profile the timeline.
4. Regulatory clock: CMN 4.935/2021 sequence, FEBRABAN cert, LGPD multi-FI consent design.
5. Per-borrower LTV (insurance attach, refi cadence) vs CAC — broker-thin vs compounding.

## 5 · What was changed on the site (same-day)

Masthead/verdict recalibrated ("structure validated — model the P&L, run the test") · 47% Honda claim decomposed · used/new financing inversion fixed · Move Motos gate corrected (R$4bn, MP 1.362 for cars) · Mexico tariff 25% · export units decoupled from e-bikes · alt-data prequal downgraded to phase-2 R&D + entrada failure-mode flagged · Candor gained the P&L-gap and adverse-selection bullets · Test gained Gate 0, Phase-0 desk sprint, realistic R1 timeline, numeric kill-gates, 8–12-loja R2, $4–6k/120-day envelope · evidence index gained this review.

**Bottom line.** The thesis survives the audit *as a structure* — Galgo-free Brazil, open correspondente supply, the composite blueprint all hold. It does not yet survive as a *business*: the P&L is unmodeled, the approval-uplift edge is contradicted by the flagship comparable, and the white space has a credible adverse-selection explanation. The corrected sequence: model the aggregator P&L (1 day, $0) → Gate 0 (local operator) → Phase-0 contract/phone sprint (2 wks, ~$200, can kill it) → only then the field test.
