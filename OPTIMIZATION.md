# Spread + Marketing Optimization: Maximizing Total Profit

## Unit Economics Baseline

At 11.75% spread, $375K ASP:

| Component | $/Unit | BPS |
|-----------|--------|-----|
| Spread | $44,100 | 1175 |
| Val Gain | $5,600 | 150 |
| Cost Structure | -$24,900 | -665 |
| LGM | $13,500 | 360 |
| Marketing | -$2,600 | -70 |
| Operations | -$4,500 | -120 |
| **PLP** | **$6,400** | **170** |

**Key insight:** Each 100 bps of spread = $3,750 per contract in margin impact.

---

## PLP by Spread Level

Holding all other costs constant, PLP at different spreads:

| Spread | BPS | PLP/Unit | Δ from 11.75% |
|--------|-----|----------|---------------|
| 9.00% | 900 | -$3,913 | -$10,313 |
| 9.50% | 950 | -$2,038 | -$8,438 |
| 10.00% | 1000 | -$163 | -$6,563 |
| **10.04%** | **1004** | **$0** | **Breakeven** |
| 10.50% | 1050 | $1,713 | -$4,688 |
| 11.00% | 1100 | $3,588 | -$2,813 |
| 11.39% | 1139 | $5,025 | -$1,375 |
| 11.75% | 1175 | $6,400 | $0 (baseline) |
| 12.00% | 1200 | $7,338 | +$938 |
| 12.39% | 1239 | $8,775 | +$2,375 |
| 13.00% | 1300 | $11,088 | +$4,688 |
| 13.39% | 1339 | $12,525 | +$6,125 |
| 14.00% | 1400 | $14,838 | +$8,438 |
| 15.00% | 1500 | $18,588 | +$12,188 |
| 16.00% | 1600 | $22,338 | +$15,938 |
| 17.00% | 1700 | $26,088 | +$19,688 |

**Critical finding:** Breakeven spread is ~10.04%. Below this, every contract loses money regardless of volume.

---

## Contracts by Spread (Extrapolated to 9%)

Using cubic spline extrapolation from 11.39%-17.39% model data:

| Spread | Contracts @ $0M | @ $20M | @ $40M | @ $60M | @ $80M |
|--------|-----------------|--------|--------|--------|--------|
| 9.00% | 26,800* | 30,400* | 32,600* | 34,800* | 36,200* |
| 9.50% | 24,600* | 27,900* | 30,000* | 32,000* | 33,400* |
| 10.00% | 22,600* | 25,600* | 27,500* | 29,400* | 30,700* |
| 10.50% | 20,700* | 23,500* | 25,300* | 27,000* | 28,100* |
| 11.00% | 19,100* | 21,600* | 23,200* | 24,800* | 25,900* |
| 11.39% | 18,485 | 21,838 | 23,514 | 25,190 | 26,028 |
| 12.39% | 15,404 | 18,198 | 19,595 | 20,992 | 21,690 |
| 13.39% | 12,837 | 15,165 | 16,329 | 17,493 | 18,075 |
| 14.39% | 10,698 | 12,638 | 13,608 | 14,578 | 15,063 |
| 15.39% | 8,915 | 10,531 | 11,340 | 12,148 | 12,552 |
| 16.39% | 7,429 | 8,776 | 9,450 | 10,123 | 10,460 |
| 17.39% | 6,191 | 7,313 | 7,875 | 8,436 | 8,717 |

*Extrapolated values - actual conversion at <11% spreads may differ

---

## Total Profit Analysis

**Total Profit = (Contracts × PLP) - Marketing Spend**

Note: PLP already includes -$2.6K marketing allocation at baseline. For different marketing spend levels, we adjust PLP:
- PLP_adjusted = PLP_base + $2.6K - (Marketing_Spend / Contracts)

### At $40M Marketing Spend:

| Spread | Contracts | PLP/Unit | Gross Profit | - Marketing | **Net Profit** |
|--------|-----------|----------|--------------|-------------|----------------|
| 9.00% | 32,600* | -$3,913 | -$128M | -$40M | **-$168M** |
| 9.50% | 30,000* | -$2,038 | -$61M | -$40M | **-$101M** |
| 10.00% | 27,500* | -$163 | -$4M | -$40M | **-$44M** |
| 10.50% | 25,300* | $1,713 | $43M | -$40M | **$3M** |
| 11.00% | 23,200* | $3,588 | $83M | -$40M | **$43M** |
| 11.39% | 23,514 | $5,025 | $118M | -$40M | **$78M** |
| **11.75%** | 22,200* | **$6,400** | **$142M** | -$40M | **$102M** |
| 12.39% | 19,595 | $8,775 | $172M | -$40M | **$132M** |
| 13.39% | 16,329 | $12,525 | $205M | -$40M | **$165M** |
| 14.39% | 13,608 | $14,838 | $202M | -$40M | **$162M** |
| 15.39% | 11,340 | $18,588 | $211M | -$40M | **$171M** |
| 16.39% | 9,450 | $22,338 | $211M | -$40M | **$171M** |
| 17.39% | 7,875 | $26,088 | $205M | -$40M | **$165M** |

---

## Profit-Maximizing Analysis

### Finding the Optimal Spread (at $40M marketing):

| Spread | Net Profit | Contracts |
|--------|------------|-----------|
| 15.39% | $171M | 11,340 |
| 16.39% | $171M | 9,450 |
| 15.00% | ~$170M | ~12,000 |
| 14.39% | $162M | 13,608 |

**Profit-maximizing spread: ~15-16%** at $40M marketing

But wait - this ignores **volume targets**. If you need contracts for market share or operational scale:

### Profit per Contract Target Analysis

What if the goal is to maximize profit while hitting a contract target?

| Contract Target | Min Spread | Max Profit | Marketing Needed |
|-----------------|------------|------------|------------------|
| 10,000 | 16.39% | $183M | $20M |
| 15,000 | 13.39% | $148M | $60M |
| 20,000 | 12.39% | $135M | $30M |
| 25,000 | 11.00%* | $50M | $60M |
| 30,000 | 10.00%* | -$45M | $80M |

**Key finding:** Above ~23,000 contracts, profit drops sharply as you enter low-margin spread territory.

---

## The Marketing ↔ Spread Trade-off

### Question: Should we reduce marketing spend and subsidize spreads instead?

Let's compare two strategies at a 20,000 contract target:

**Strategy A: Higher Marketing, Higher Spread**
- Spread: 13.39%
- Marketing: $80M
- Contracts: ~19,500
- PLP: $12,525
- **Net Profit: $244M - $80M = $164M**

**Strategy B: Lower Marketing, Lower Spread**
- Spread: 12.00%
- Marketing: $20M
- Contracts: ~20,000
- PLP: $7,338
- **Net Profit: $147M - $20M = $127M**

**Strategy A wins by $37M** despite higher marketing spend, because the PLP is so much higher.

### The Crossover Point

When does spread subsidy beat marketing spend?

For 100 bps spread reduction:
- Margin cost: $3,750 × Contracts
- At 20,000 contracts: $75M annual margin impact

This must be offset by marketing savings. Marketing efficiency at different levels:

| Marketing Reduction | Contracts Lost | Cost per Contract Saved |
|--------------------|----------------|------------------------|
| $80M → $60M | ~1,500 | $13,333 |
| $60M → $40M | ~1,800 | $11,111 |
| $40M → $20M | ~2,500 | $8,000 |
| $20M → $0M | ~3,500 | $5,714 |

**To break even on 100 bps spread reduction:**
- Need to save $75M in marketing
- Would need to cut marketing from ~$90M to ~$15M
- But that loses ~6,000 contracts
- So you'd need the spread reduction to generate >6,000 contracts

At 13% → 12% spread:
- Contract gain: ~3,300 (at $40M spend)
- Not enough to offset the volume loss from cutting marketing by $75M

**Conclusion: At current economics, marketing spend is more efficient than spread subsidy for hitting volume targets.**

---

## Optimal Strategy by Objective

### Objective: Maximize Profit (volume flexible)
- **Optimal: 15-16% spread, $40-60M marketing**
- Delivers: ~$170M profit, ~10-12K contracts

### Objective: Maximize Contracts (profit flexible)
- **Optimal: 11% spread, $80M+ marketing**
- Delivers: ~25K contracts, ~$50M profit

### Objective: Balanced (15K+ contracts, maximize profit)
- **Optimal: 13-14% spread, $40-60M marketing**
- Delivers: ~$160M profit, ~15-17K contracts

### Objective: Growth Mode (20K+ contracts, stay profitable)
- **Optimal: 12% spread, $40M marketing**
- Delivers: ~$130M profit, ~20K contracts

---

## Critical Constraints

1. **Breakeven spread is ~10%** - Below this, every contract loses money
2. **Contracts are capped by spread** - At 17% spread, max ~10K contracts regardless of marketing
3. **Marketing ROI drops sharply above $60M** - Diminishing returns accelerate
4. **Spread has higher profit leverage than volume** - 100 bps = $3,750/contract vs ~$1,500 profit impact from 1,000 more contracts

---

## Recommendation

**Do NOT trade marketing dollars for spread subsidy below 12%.**

The math doesn't work:
- Each 100 bps below 12% costs $3,750/contract in margin
- The volume gains don't offset the margin loss
- You hit profitability danger zone below 11%

**Instead:**
1. Set spread at 12-13% for balance of volume and margin
2. Allocate $40-60M to marketing (efficient zone)
3. Use spread tactically (market-by-market) rather than blanket reduction
4. Reserve spread subsidies for high-LTV or strategic segments only

