# Financial reporting in Power BI

Two finance reports I built in Power BI during my MSc at Audencia (Financial Data Visualization course).
Open the `.pbix` files in [Power BI Desktop](https://www.microsoft.com/power-bi/desktop) (free).

## 1. Group financial statements: 7 subsidiaries, 3 regions

`financial-statements/financial_statements.pbix`

**Question:** how are sales, profitability and working capital developing across a group with 7 subsidiaries,
and what drives the change in net income?

**Data:** a general ledger for 7 entities (Brazil, Canada, France, Germany, Spain, UK, USA) in 3 regions
(Europe, North America, South America), 2022 to 2024, mapped to a 54-account chart of accounts.

**Model:** star schema built in Power Query (fact: general ledger; dimensions: date, entity, chart of accounts),
with a date table and DAX measures.

| Page | What it shows |
|---|---|
| Sales Analysis | Revenue by entity and country, year → quarter → month drill-down, sales growth % |
| Projected Sales by Country | 2025 projection per country, using the 2024 vs 2023 growth rate |
| Income Statement | Full P&L down to net income |
| Balance Sheet | Assets vs equity and liabilities, by year |
| KPIs | Gross margin %, operating profit %, EBIT, EBITDA %, net income % |
| KPI cards | DIO, DPO, DSO and cash conversion cycle |

## 2. FMCG P&L variance for the CFO and CEO

`fmcg-pl-variance/`

**Question:** where did profit move against last year, budget and forecast, and was it volume or price/mix?

**Data:** an FMCG company's 2020-2021 actuals, 2021 budget and a 6+6 forecast (67,000+ rows).

| File | Pages |
|---|---|
| `fmcg_pl_vs_budget_forecast.pbix` | P&L (actual vs last year, budget and forecast, with € variances), per-kg KPIs (gross sales, net sales, cost of production and distribution per kg), operating profit waterfall |
| `fmcg_price_mix_volume.pbix` | P&L by brand and category with variance vs budget and last year (value and %), sales price/mix vs volume effect, waterfall bridge, KPI cards (net sales per kg, operating profit %) |

## Skills

Power BI, Power Query, DAX, star-schema data modelling, financial statements, variance analysis,
price/volume/mix analysis, working capital KPIs.
