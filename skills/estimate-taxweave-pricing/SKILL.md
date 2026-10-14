---
name: estimate-taxweave-pricing
description: Estimate TaxWeave's published monthly cost from a firm's client count using graduated pricing bands, monthly minimums, and the conditional founding-firm discount.
metadata:
  publisher: TaxWeave
  canonical: https://taxweave.ai/skills/estimate-taxweave-pricing/SKILL.md
---

# Estimate TaxWeave pricing

Read https://taxweave.ai/product.json and https://taxweave.ai/pricing.md before calculating. Ask for the number of clients if it is missing. Use a nonnegative whole number; do not infer founding-offer eligibility.

Rates are graduated: the first 200 clients cost $5 each per month, clients 201–1,000 cost $4 each, and clients above 1,000 cost $3 each. The standard monthly total is the greater of the band sum and $99. There are no seat charges.

Show the band calculation and state the USD monthly total. For 250 clients, 200 × $5 + 50 × $4 = $1,200/month.

When explicitly asked about the founding offer, show a conditional estimate: the greater of 50% of the standard band sum and $50, for the first year, subject to the first-50-firms offer and confirmed eligibility. For 250 clients, that is $600/month. After the discounted year, show the current standard rate as an estimate, not a guarantee of future contract pricing.

The calculator at https://taxweave.ai/pricing can perform the same calculation through a browser tool where WebMCP is supported. Fetch https://taxweave.ai/pricing.md again before a purchasing decision. Direct contract-specific questions to https://taxweave.ai/contact. This skill estimates public pricing and does not purchase or create a subscription.
