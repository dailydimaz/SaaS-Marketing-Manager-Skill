# SaaS Marketing Manager Skill

A Codex or Claude skill for practical SaaS marketing work: growth strategy, acquisition channels, lifecycle marketing, retention, positioning, go-to-market planning, and KPI diagnosis.

The skill is written to behave like a senior SaaS marketing manager. It turns vague goals such as "grow sign-ups" or "improve free-to-paid conversion" into focused, metric-driven recommendations and finished marketing assets.

## When To Use It

Use this skill when you want help with:

- Growth strategy for SaaS, PLG, freemium, or B2B software products
- Channel selection across SEO, content, paid, community, partnerships, and product-led loops
- Activation, onboarding, lifecycle emails, and free-to-paid conversion
- Churn reduction, retention analysis, reactivation, and expansion
- Positioning, messaging, competitor analysis, and differentiation
- Go-to-market planning for a product, feature, or new segment
- SaaS KPIs, funnel diagnosis, dashboards, and metric interpretation

Example prompts:

```text
Build a 90-day growth plan for our PLG SaaS.
Improve free-to-paid conversion for our freemium product.
Write an onboarding email sequence for new sign-ups.
Position our product against a larger competitor.
Diagnose why sign-ups are not turning into paid users.
Create a launch plan for a new analytics feature.
```

## How The Skill Thinks

The skill anchors recommendations to the SaaS funnel:

```text
Awareness -> Acquisition -> Activation -> Revenue -> Retention -> Referral
```

It prioritizes work by asking:

- Which funnel stage is the real bottleneck?
- Which metric should this work move?
- Is the product motion PLG, self-serve, freemium, or sales-led?
- Which 1-3 bets are worth doing now?
- What should be ignored until the current constraint is fixed?

The skill is intentionally execution-oriented. For asset requests, it should produce the actual email, campaign plan, launch sequence, positioning statement, or dashboard structure instead of stopping at theory.

## Repository Structure

```text
.
|-- SKILL.md
|-- README.md
|-- LICENSE.txt
`-- references/
    |-- channels-and-growth.md
    |-- lifecycle-and-retention.md
    |-- metrics-and-kpis.md
    `-- positioning-and-gtm.md
```

File roles:

- `SKILL.md` is the skill entry point. It contains the trigger description, operating principles, funnel model, and guidance on when to read each reference file.
- `references/channels-and-growth.md` covers acquisition channel selection, growth loops, PLG distribution, and growth plan structure.
- `references/lifecycle-and-retention.md` covers activation, onboarding, free-to-paid conversion, churn, reactivation, and expansion.
- `references/metrics-and-kpis.md` defines SaaS metrics, funnel dashboards, CAC/LTV/payback, churn, NRR, and honest metric interpretation.
- `references/positioning-and-gtm.md` covers positioning, messaging, competitive differentiation, localization, and launch planning.

## Installation

Install it as a Codex skill by placing this directory in your Codex skills folder:

```bash
mkdir -p ~/.codex/skills
cp -R /path/to/SaaS-Marketing-Manager-Skill ~/.codex/skills/saas-marketing-manager
```

After installation, Codex can trigger the skill automatically when a request matches the description in `SKILL.md`.

## Customization

To adapt the skill:

- Edit the `description` in `SKILL.md` to broaden or narrow when the skill triggers.
- Add more reference files under `references/` for industry-specific playbooks.
- Update the "What this role owns" table in `SKILL.md` if you add new reference areas.
- Keep guidance practical, metric-linked, and tied to SaaS funnel stages.

Good additions include examples from your own market, preferred KPI definitions, pricing and packaging rules, ICP-specific messaging, or localized acquisition channels.

## License

MIT. See `LICENSE.txt`.
