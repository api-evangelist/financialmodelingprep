# Financial Modeling Prep (financialmodelingprep)

Financial Modeling Prep (FMP) is a financial data API provider offering real-time and historical market data, company fundamentals, and regulatory filings through more than 100 REST endpoints plus real-time WebSocket streams. Coverage includes income statements, balance sheets, and cash-flow statements; stock, ETF, index, forex, crypto, and commodity quotes; up to 30 years of historical prices; SEC filings (10-K, 10-Q, 8-K); analyst estimates and price targets; key metrics, ratios, and enterprise values; and macroeconomic indicators such as GDP, treasury rates, and inflation.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/apis.yml)

## Access Model

- **Public, key-authenticated REST API.** Every request carries an API key as the `apikey` query parameter, e.g. `?apikey=YOUR_API_KEY`. Self-service signup issues a key.
- **Stable base:** `https://financialmodelingprep.com/stable`. A legacy base, `https://financialmodelingprep.com/api/v3` (and `/api/v4`), is still documented and in wide use.
- **Formats:** JSON by default; most endpoints also return CSV via a `datatype` parameter.
- **Real-time WebSocket** streams (`wss://`) are available for stocks, crypto, and forex on real-time-eligible plans.
- **Free tier:** the Basic plan allows up to **250 requests per day** against end-of-day / sandbox data. Paid tiers add real-time coverage, higher per-minute rate limits, larger bandwidth allowances, deeper history, more markets, and premium datasets.

Endpoint paths, exact rate limits, and bandwidth allowances in this repository are grounded in FMP's public documentation as of the review date. Monthly and annual **prices are not reconciled** here and should be verified on the FMP pricing page before use, as tiers and prices change over time.

## Tags

- Financial Data
- Market Data
- Fundamentals
- SEC Filings
- Stocks
- Economic Indicators
- Quotes
- Regulatory Filings

## Timestamps

- **Created:** 2026-07-11
- **Modified:** 2026-07-11

## APIs

### Financial Modeling Prep Financial Statements API

Audited annual and quarterly financial statements for public companies - income statement, balance sheet, and cash-flow statement - with extensive historical coverage and both as-reported and trailing-twelve-month (TTM) formats.

- **Human URL:** [https://site.financialmodelingprep.com/developer/docs/stable](https://site.financialmodelingprep.com/developer/docs/stable)
- **Base URL:** `https://financialmodelingprep.com/stable`

### Financial Modeling Prep Quotes and Prices API

Real-time and delayed quotes for stocks, ETFs, mutual funds, indexes, forex, crypto, and commodities across major global exchanges, plus end-of-day and intraday historical prices with up to 30 years of dividend-adjusted history.

- **Human URL:** [https://site.financialmodelingprep.com/developer/docs/stable](https://site.financialmodelingprep.com/developer/docs/stable)
- **Base URL:** `https://financialmodelingprep.com/stable`

### Financial Modeling Prep SEC Filings API

Real-time access to the latest SEC filings submitted by public companies, searchable by ticker symbol or CIK and by date range. Covers 10-K, 10-Q, 8-K, and other form types with links to the source EDGAR documents.

- **Human URL:** [https://site.financialmodelingprep.com/developer/docs/stable/financials-latest](https://site.financialmodelingprep.com/developer/docs/stable/financials-latest)
- **Base URL:** `https://financialmodelingprep.com/stable`

### Financial Modeling Prep Fundamentals API

Company profiles plus derived fundamentals - key metrics, financial ratios, enterprise values, financial scores, and owner-earnings - computed from the underlying statements and served per ticker for screening and valuation.

- **Human URL:** [https://site.financialmodelingprep.com/developer/docs/stable](https://site.financialmodelingprep.com/developer/docs/stable)
- **Base URL:** `https://financialmodelingprep.com/stable`

### Financial Modeling Prep Analyst Estimates API

Consensus analyst estimates for revenue, EPS, and other forecast figures, together with analyst price targets and stock grades / rating changes.

- **Human URL:** [https://site.financialmodelingprep.com/developer/docs/stable/financial-estimates](https://site.financialmodelingprep.com/developer/docs/stable/financial-estimates)
- **Base URL:** `https://financialmodelingprep.com/stable`

### Financial Modeling Prep Economic Data API

Macroeconomic indicators such as GDP, inflation (CPI), unemployment, and retail sales, plus U.S. treasury rates and a forward-looking economic calendar.

- **Human URL:** [https://site.financialmodelingprep.com/developer/docs/stable](https://site.financialmodelingprep.com/developer/docs/stable)
- **Base URL:** `https://financialmodelingprep.com/stable`

### Financial Modeling Prep Real-Time WebSocket API

Real-time streaming market data over WebSocket for stocks, crypto, and forex. Clients connect, send a login event carrying their API key, then subscribe to tickers to receive top-of-book quote and last-trade messages as they occur.

- **Human URL:** [https://site.financialmodelingprep.com/datasets/websocket](https://site.financialmodelingprep.com/datasets/websocket)
- **Base URL:** `wss://websockets.financialmodelingprep.com`

## Common Properties

- [Authentication](authentication/financialmodelingprep-authentication.yml)
- [GitHub Organization](https://github.com/FinancialModelingPrepAPI)
- [LinkedIn](https://www.linkedin.com/company/financial-modeling-prep)
- [Website](https://site.financialmodelingprep.com/)
- [Documentation](https://site.financialmodelingprep.com/developer/docs/stable)
- [Plans](plans/financialmodelingprep-plans-pricing.yml)
- [Rate Limits](rate-limits/financialmodelingprep-rate-limits.yml)
- [Fin Ops](finops/financialmodelingprep-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
