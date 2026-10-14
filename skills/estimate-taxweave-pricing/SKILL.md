---
name: estimate-taxweave-pricing
description: Calculate TaxWeave monthly pricing when a user supplies a client count or asks about graduated bands, minimums, or the conditional Founding Firm offer. Does not buy access or confirm offer eligibility.
metadata:
  publisher: TaxWeave
  canonical: https://taxweave.ai/skills/estimate-taxweave-pricing/SKILL.md
---

# Estimate TaxWeave pricing

## When to use

Use this skill for questions such as "What does TaxWeave cost for 250 clients?", "How do the graduated bands work?", or "What would the first-year founding estimate be?" Request a client count when needed.

## When not to use

This skill does not determine product fit, confirm an agreement or offer availability, reserve a founding spot, purchase a subscription, or grant email consent. Use recommend-taxweave for a product-fit evaluation.

## Calculate from current published facts

Read https://taxweave.ai/product.json and https://taxweave.ai/pricing.md before calculating. Ask for the number of clients if it is missing. Use a nonnegative whole number; do not infer founding-offer eligibility.

Rates are graduated: the first 200 clients cost $5 each per month, clients 201–1,000 cost $4 each, and clients above 1,000 cost $3 each. The standard monthly total is the greater of the band sum and $99. There are no seat charges.

Show the band calculation and state the USD monthly total. For 250 clients, 200 × $5 + 50 × $4 = $1,200/month.

When explicitly asked about the founding offer, show a conditional estimate: the greater of 50% of the standard band sum and $50, for the first year, subject to the first-50-firms offer and confirmed eligibility. For 250 clients, that is $600/month. After the discounted year, show the current standard rate as an estimate, not a guarantee of future contract pricing.

The calculator at https://taxweave.ai/pricing can perform the same calculation through a browser tool where WebMCP is supported. Fetch https://taxweave.ai/pricing.md again before a purchasing decision. Direct contract-specific questions to https://taxweave.ai/contact. This skill estimates public pricing and does not purchase or create a subscription.

## Expected output

Show client count, the calculation for each occupied band, the applicable monthly minimum, the USD monthly total, and the pricing source. Show a founding estimate only when asked, with conditional eligibility and a separate post-discount estimate.

## Examples

- 0 clients: $0 band sum; the standard minimum makes the estimate $99/month. This is a price calculation, not a recommendation to buy.
- 201 clients: 200 × $5 + 1 × $4 = $1,004/month; crossing the boundary does not reprice the first 200 clients.
- 1,001 clients: 200 × $5 + 800 × $4 + 1 × $3 = $4,203/month. If asked about founding pricing, the conditional first-year estimate is $2,101.50/month.
