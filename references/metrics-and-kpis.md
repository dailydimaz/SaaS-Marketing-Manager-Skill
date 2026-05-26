# Metrics & KPIs

A SaaS marketing manager lives in the dashboard. Numbers are how you choose between bets, prove what worked, and avoid fooling yourself. The key skill: know which metrics matter, and interpret them honestly — most marketing failures hide behind a flattering vanity number.

---

## The metric stack, mapped to the funnel

| Funnel stage | Key metrics | What it tells you |
|---|---|---|
| Awareness | Traffic, reach, impressions | Top-of-funnel volume (leading; easily vanity) |
| Acquisition | Sign-up rate, **CAC** | Converting attention into accounts, and at what cost |
| Activation | **Activation rate**, time-to-activation | Are sign-ups reaching first value? (the real bottleneck) |
| Revenue | Free-to-paid %, **MRR/ARR**, ARPU | Converting value into recurring revenue |
| Retention | **Churn rate**, retention curve, **NRR** | Keeping and growing the base |
| Referral | Viral coefficient (k), referral rate | Does the product/loop spread itself? |

**Bolded = the metrics that actually drive decisions.** Watch leading indicators (sign-up rate, activation) weekly — they move fast and predict the lagging ones (MRR, churn) that prove the outcome.

---

## Core metrics — defined plainly

### CAC (Customer Acquisition Cost)
- **Formula:** Total sales + marketing spend ÷ new customers acquired in same period
- **Judge channels on CAC per activated user**, not cost-per-click
- A channel with high CPC but great conversion can be cheaper on CAC than a "cheap" channel that converts poorly

### LTV (Lifetime Value)
- **Formula:** ARPU ÷ churn rate (margin-adjusted for accuracy)
- The ceiling on what you can spend to acquire a customer
- Rule of thumb: **LTV:CAC ≥ 3:1** is healthy; below 1:1 you lose money on every customer

### CAC Payback Period
- **Formula:** CAC ÷ monthly gross margin per customer
- How many months until a customer's margin repays their CAC
- Short payback = reinvest faster; long payback strains cash even if LTV:CAC looks fine

### Activation Rate
- **Formula:** % of sign-ups who reach the defined activation event
- The most under-watched, high-leverage number in the stack
- A 10pp improvement in activation rate often outperforms a 30% increase in sign-up volume

### MRR / ARR (Monthly/Annual Recurring Revenue)
- The heartbeat of a SaaS business
- **Break MRR growth into components:**
  ```
  New MRR (new customers)
  + Expansion MRR (upgrades, upsell)
  − Churned MRR (cancellations)
  − Contraction MRR (downgrades)
  = Net new MRR
  ```
  Where growth comes from matters as much as the total

### Churn
- **Logo churn:** % of customers lost per period
- **Revenue churn:** % of MRR lost per period (matters more — one big account ≠ one small account)
- Calculate monthly; annualize for benchmarking

### NRR (Net Revenue Retention)
- **Formula:** (Revenue from last period's customers this period, including expansion) ÷ (Revenue from those customers last period) × 100
- **NRR > 100% = existing base grows on its own** — even with zero new acquisition
- The strongest signal of product-market fit; worth setting as a north-star goal
- Best-in-class SaaS: 120–140%+ NRR

---

## How the metrics chain together

Don't read in isolation — read the chain:

```
More sign-ups × better activation rate
    → more activated users
    → higher retention (activated users retain dramatically better)
    → higher LTV
    → higher affordable CAC
    → unlocks more/bigger acquisition channels
```

And from the retention side:
```
Better retention → higher NRR
→ revenue grows without acquisition spending
→ lower growth requirement from marketing
→ more margin to invest in product
```

**When diagnosing, walk *down* the funnel** to find the first stage that's leaking. The named symptom is usually downstream of the real problem.

---

## Reading numbers honestly

- **Vanity vs. actionable.** Impressions/followers/clicks feel good and decide nothing. Always push to the nearest metric tied to sign-ups or revenue.
- **Correlation ≠ attribution.** "We blogged and sign-ups rose" may be coincidence. Prefer controlled tests; treat last-click attribution as a hint, not truth.
- **Averages hide cohorts.** Blended CAC and average retention mask huge channel/segment differences. Segment before concluding.
- **Timing and compounding.** SEO/content looks broken early, great late. Paid looks great while subsidized, worse at scale. Don't extrapolate naively or kill a channel on a 6-week read.
- **Guardrail metrics.** When optimizing one number, name the one you must not harm (e.g., lifting free-to-paid by gutting the free tier can tank total sign-ups and viral spread). Win the metric without breaking the funnel.

---

## Dashboard design

When asked to design a marketing dashboard:

### Executive view (north-star, weekly)
- MRR + MRR growth %
- CAC (blended) and CAC payback period
- Activation rate
- Churn rate and NRR
- Free-to-paid conversion %

### Operating view (channel-level, for the marketing team)
- Traffic by channel + sign-up rate per channel
- Activation rate by cohort/acquisition source
- Email open/click/conversion rates per sequence step
- Paid: CPC, conversion rate, CAC per channel

**Always show trend over time** — a number without its trend is nearly useless. Pair each metric with the action it would trigger if it moved in either direction.

If asked to build the dashboard, offer an interactive HTML/React dashboard with trend lines — it beats a static table for day-to-day use.
