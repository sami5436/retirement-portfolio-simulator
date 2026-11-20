# Portfolio Atlas — Retirement Portfolio Simulator

Next.js mobile-first retirement backtesting app for S&P 500, FSELX, bonds, QQQ, SCHD, JEPQ, JEPI or up to 15 Yahoo Finance tickers.

## Features
- Custom Yahoo Finance tickers and historical date range
- Preset 100/0, 80/20, 60/40, 40/60, semiconductor and dividend allocations; custom percentage sliders
- $500,000 default capital, monthly 4% initial withdrawal increased with annual inflation or 4% variable portfolio withdrawals
- 10-, 20- and 30-year historical backtests; missing historical funds shown as N/A
- Monte Carlo 500-path 12-month correlated block resampling, annual rebalancing, distribution snapshots, simplified tax drag, CSV exports
- Mobile-first dark interface

## Local development
Node 20+ required.

```bash
npm install
npm run dev
```

Deploy by connecting the repository to Vercel with Next.js framework. No API key required; Yahoo Finance chart is unofficial and rate-limits may apply.

## Important qualifications
Adjusted closing prices include distributions; distributions are not double-counted. Data date ranges are limited by fund inception and shared historical coverage. Monte Carlo is not a forecast. Tax drag uses illustrative flat rates, not full federal tax brackets, state tax, specific account treatment, or tax-lot accounting. No fees or transaction costs.