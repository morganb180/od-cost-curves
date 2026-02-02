# Marketing Cost Curves

Interactive visualization of marketing spend vs contracts with diminishing returns analysis.

**[Key Findings →](FINDINGS.md)** | **[Spread vs Spend Arbitrage →](ARBITRAGE.md)** | **[Profit Optimization →](OPTIMIZATION.md)**

## Features

- **Diminishing Returns Curves**: 7 spread levels showing contracts by marketing spend
- **Custom Spread Interpolation**: Add any spread level (e.g., 11.27%, 9.5%) using 2D cubic spline interpolation
- **Marginal CAC Table**: Cost per incremental contract at each $5M tranche
- **Incremental CAC Table**: Blended cost across all marketing spend
- **Flexible Display**: Toggle between $ amounts and % of home price
- **Dev Mode**: View underlying data, formulas, and interpolation calculations

## Usage

Open `index.html` in a browser. No build step required.

## Data Source

GTM (Growth Toy Model) sensitivity tables - Base 2026 case.

## Color Thresholds

Based on % of average home price:
- **Green (efficient)**: ≤2%
- **Yellow (moderate)**: 2-4%
- **Red (expensive)**: >4%
