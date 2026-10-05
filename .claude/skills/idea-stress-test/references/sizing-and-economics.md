# Sizing and unit economics

Rules of thumb for the Market, Distribution, and Unit economics sections. The benchmarks below are **starting heuristics, not facts**. When a number drives the verdict, search for a current source and cite it, or label it clearly as an assumption.

## Bottom-up market sizing

Always show the arithmetic as a chain the user can challenge link by link.

**B2B:**
```
# of target accounts (define the segment precisely + source for the count)
× % that have the problem acutely enough to buy (assumption, justify)
× realistic ACV (anchor to what they pay for adjacent tools today)
= serviceable market
→ realistic 5-year capture (typically 5–15% for a strong startup) = revenue ceiling
```

**Consumer:**
```
# of people with the problem in reachable geos
× % reachable via the channels you'll actually use
× install → active conversion
× active → paid conversion
× annual revenue per paying user
= revenue potential
```

**Rebuilding an inflated top-down TAM:**
1. Quote the claim ("Deck: $8bn programmatic analytics TAM, we need 1%").
2. Identify what the big number actually measures (often total category *spend*, not spend on *this kind of tool*).
3. Rebuild bottom-up as above.
4. State the gap as a ratio and say what it means: "Bottom-up ≈ $60M serviceable — fine for a $5–10M ARR business, not obviously venture-scale. That's a fundraising-strategy question, not necessarily a kill."
5. Note venture-scale threshold: for VC-backed, ask whether the serviceable market plausibly supports $100M+ ARR. If not, say so, and point out it can still be a good bootstrapped business.

## Distribution: first 10 / 100 / 1,000

| Stage | Typical channel | What to state |
|---|---|---|
| First 10 | Founder network, ex-colleagues, direct outreach, communities the founder is already in | Which specific types of people/companies, and how the founder reaches them this month |
| First 100 | Outbound, content, partnerships, referrals, targeted paid | Repeatable channel + rough conversion rates + CAC estimate |
| First 1,000 | Scaled paid, channel partners, product-led growth, marketplace/app store | Which channel scales, and whether CAC holds as it does |

Flag when the first 10 rely on the founder's personal network but there's no story for 11–100.

## Unit-economics checks

Compute and show, with assumptions:

- **Gross margin** = (revenue − cost to serve) / revenue. Cost to serve includes infra, third-party data/API costs, LLM inference, payment fees, and *human* onboarding/support/services.
  - Software-like businesses are usually expected at roughly 70–80%+. Below ~60%, investors tend to value it as services or a marketplace; say so.
  - AI products: model inference cost per user/action × usage. Flag usage-heavy users who could go margin-negative on flat pricing.
- **CAC** = fully loaded sales + marketing spend / new customers. For founder-led sales, cost the founder's time.
- **CAC payback (months)** = CAC / (monthly revenue per customer × gross margin). Common heuristics: < 12 months good for SMB/mid-market, < 18–24 acceptable for enterprise.
- **LTV/CAC** — only meaningful once there's retention data; until then, mark the retention input as a Hope.

## Pattern library

### B2B data / ad-tech
Pressure points to always check:
- **Who captures value in the chain.** If the product raises publisher yield, does the publisher pay, or does the SSP/DSP absorb it? Take-rate products compete with intermediaries that already take a cut.
- **Sales cycle and procurement.** Large publishers, holding companies, and brands have legal, security, and privacy review. A pilot-to-contract cycle of 6–12 months can kill a capital-light founder; size runway against it.
- **Platform dependency.** Google (Ad Manager, Chrome, Privacy Sandbox status), Amazon, The Trade Desk, Apple (ATT). Ask: what happens if one of them changes a policy or ships this as a feature? Search for current status rather than relying on memory, as this changes often.
- **Data rights and privacy.** Who owns the data, what consent covers this use, and how GDPR, state privacy laws, and clean-room terms constrain it.
- **Services creep.** Ad-tech "SaaS" often hides heavy managed service. Check gross margin with real support hours.
- **Founder-market fit lever.** The user's network of publisher and agency contacts is a real distribution asset for the first 10. Say so where true, but test whether it extends past 10.

### Small consumer apps (solo, capital-light)
Pressure points to always hammer:
- **Distribution is usually the business.** App-store search is crowded; paid installs often cost $2–5+ per install in competitive categories (verify for the category). Ask: is there an organic channel the founder controls (audience, community, SEO surface, built-in virality)?
- **Retention.** Most consumer apps lose the large majority of installs within 30 days. Ask for (or set as a pass/fail threshold) D1 / D7 / D30 retention targets *before* building. For habit apps specifically, motivation decays and novelty wears off. What brings people back on day 15?
- **Willingness to pay.** Large free and incumbent alternatives exist in most categories. Typical install → paid conversion is in the low single-digit %. Do the arithmetic: how many installs are needed to reach $X MRR, and what does that cost?
- **Platform fees.** App stores take 15–30%. Include in margin.
- **Solo-founder bandwidth.** Building, marketing, support, and iteration on nights and weekends. Which one gets dropped?
- **Founder-market fit.** An ad-tech PM background helps with paid acquisition literacy and measurement, but not with consumer product taste or content. Be honest.

Example cheap tests for consumer:
- Fake-door landing page + $200 of targeted ads → pass = email signup rate ≥ X% at CPC ≤ $Y.
- Concierge version (spreadsheet, group chat, or Notion template) with 20 users for 2 weeks → pass = ≥ 40% still engaging on day 14 without nudges.
- Pre-sale: "founding member" price via Stripe link → pass = ≥ N paid before writing code.
