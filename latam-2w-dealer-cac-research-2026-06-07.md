---
type: report
topic: "LatAm Moto Dealer CAC — what it costs a dealer to acquire a buyer"
date: "2026-06-07"
method: "4-agent parallel research sweep (Meta/CTWA + marketplace + dealer mix + lead-gen/finance)"
confidence: "medium (directional; country×moto×CTWA cells are thin)"
related:
  - "[[latam-2w-leadgen-markets]]"
  - "[[latam-2w-leadgen-business-model-validation-2026-06-06]]"
---

# LatAm Moto Dealer CAC — Research Synthesis (2026-06-07)

**Why this matters:** the dealer's own cost-to-acquire a buyer is the *real* ceiling on what a lead-gen intermediary can charge (`price ≤ min(ROI limit, dealer's own CAC)`). It was the single biggest guessed input in the [[latam-2w-leadgen-business-model-validation-2026-06-06|business-model validation]]. A 4-agent web sweep grounded it.

## Headline numbers (USD, Brazil/Colombia/Mexico, 2024–25)

| Component | Estimate | Confidence |
|---|---|---|
| **Dealer self-serve Meta CTWA** (qualified lead) | **$4–7** competent · ~$8 amateur | med |
| **Marketplace effective CPL** (Webmotors, iCarros, Mercado Libre, TuCarro) | **$4–8** (quality poor, ~5% convertible) | med (BR), low-med (MX/CO) |
| **Organic / walk-in / referral share** of moto-dealer sales | **~50%** (40–60%) | low-med |
| **Implied dealer CAC per sale** (moto) | **~$100–350** | low |
| **Lead→sale conversion** — general internet | **~6%** (2–10%) | high |
| **Lead→sale conversion** — Brazil WhatsApp, <1 min reply | **~20%** (decays to ~10% @1h, ~1% @24h) | med-high |
| **Finance origination commission** (correspondente bancário, BR) | **2–5% of loan = $45–175/moto loan** | med |
| **Consórcio admin fee** (motos, BR) | **15–20% of credit** (revenue pool for seller commissions) | high |
| **Dealer marketing spend** | ~1–2% of revenue; ~$150–400/unit (moto) | med (US-anchored) |

## The central implication: arbitrage compression

The dealer's self-serve CTWA cost (~$5 competent) is **≈ our own ~$5 CAC** — both buy from the **same Meta auction**. So the pure per-lead arbitrage is **near zero**. The business only exists three ways:
1. **Beat an amateur dealer** — a small dealer runs ads badly (~$8–10); a specialist hits ~$5 → a real ~$3–5 arbitrage. *Erodable.*
2. **Speed-to-lead conversion** — fast WhatsApp (~20%) vs a dealer's slow follow-up (~6%). Sub-minute response is the operational moat.
3. **Finance-qualification + origination** — the uncapped second revenue stream ($45–175/loan) they can't replicate. The real defensibility.

## Who pays / who doesn't

- **Pays:** demand-gen-starved dealers & new Chinese brands — bad at their own ads, short on organic. (Matches the long-tail-entrant thesis.) Use as a **pitch filter**.
- **Doesn't:** established dealers with organic flow or in-house marketing — their make-cost ≤ our CAC → no deal.

## What it changed in the model

The validation calculator was rewired: price ceiling = `min(ROI limit, dealer self-serve CAC)`; dealer revenue haircut by organic share; new sliders for **dealer's own CAC ($8 default)** and **organic % (50% default)**. At researched defaults (self-serve $8, organic 50%, conv 6%) the base case is **marginally negative (−$0.10/lead)** — it only flips positive on higher conversion (fast WhatsApp), less organic, higher-margin bikes, or the financing stream. This is the honest, data-grounded picture.

## Caveats

- Country×moto×CTWA benchmarks are thin; most figures interpolate global-auto onto LatAm CPM/CPC. Treat as ranges.
- Marketplace per-lead is *derived* (plan ÷ leads/listing), not a published sold-lead SKU — a real data gap (verify a Webmotors sold-lead price in Phase 1).
- Moto-specific origination commission & attach rate are the weakest points — flag for primary-source follow-up (Banco PAN, BV, Santander Financiamentos disclosures).
- Organic "~50% of sales" is a TAM signal, not a literal 1:1 per-lead haircut; the calculator models it conservatively.

## Sources (top, by agent)

- **Paid ads:** AdAmigo (Meta CPM/CPC by country), WordStream/LocaliQ (auto benchmarks), AsisteClick (CTWA LatAm), Statista (Google CPC LatAm).
- **Marketplaces:** Webmotors "Quanto custa vender", iCarros plans, Mercado Libre MX exposure pricing, TuCarro CO listing costs.
- **Dealer mix/spend:** Hrizn (dealer marketing budget), DemandLocal (CAC by vehicle type), AutoForce (BR 400-dealer digital study), Think-with-Google Gearshift.
- **Lead-gen/finance:** US auto/subprime lead pricing, DemandLocal conversion stats, Intelia (BR WhatsApp conversion), Procon/InfoMoney (BR "taxa de retorno" commission), Banco PAN / Ademicon (moto finance & consórcio).
