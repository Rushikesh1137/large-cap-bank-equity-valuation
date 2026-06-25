# Large-Cap Bank Equity Valuation: JPMorgan Chase

A self-directed equity valuation of JPMorgan Chase & Co. (NYSE: JPM), focused on how banks are valued through equity, book value, and return on equity rather than enterprise value.

**Rating: Neutral / Hold - Target ~$324 - Price ~$334**

## Overview

This project asks a practical equity-research question: is the best-run US large-cap bank worth buying at today's price? The answer from the model is cautious. JPMorgan is a high-quality bank with FY2025 ROE of about 17%, ROTCE of about 20%, and a CET1 ratio of about 14.6%, but the market price already gives it credit for those strong returns.

The repository contains two core deliverables:

| File | Purpose |
| --- | --- |
| [JPM_Model_Lite.xlsx](model/JPM_Model_Lite.xlsx) | Four-year historical model and justified price-to-book valuation. |
| [JPM_Research_Note.pdf](research-note/JPM_Research_Note.pdf) | Two-page research note summarizing the valuation view. |

## Why Banks Are Valued Differently

For a normal company, debt is financing. Analysts often value the whole enterprise using discounted free cash flow or multiples like EV/EBITDA, then subtract net debt to reach equity value.

For a bank, deposits and borrowings are raw material. They are the inputs the bank lends out, not just financing. Because of that, enterprise value and free cash flow are not clean measures for bank valuation. Banks are usually valued directly on equity using methods such as price-to-book versus return on equity, residual income / justified P/B, and dividend or total-payout models.

## The Model

The spreadsheet has three tabs:

| Tab | What it does |
| --- | --- |
| `Read Me` | Explains the model scope and the input/formula convention. |
| `Model` | Holds FY2022-FY2025 historical results and computed ratios. |
| `Valuation` | Applies the justified P/B framework to JPM's FY2025 book value. |

The model uses a clear color convention: blue cells are reported facts, while black cells are formulas. Reported inputs include revenue, expense, provision, net income, share counts, and book value. Derived items include noninterest revenue, pre-provision profit, pre-tax income, tax expense, EPS, common and tangible equity, ROE, ROTCE, efficiency ratio, credit cost, and the valuation output.

Changing a blue input should flow through the rest of the model through formulas.

## Valuation Method & Result

The core method is justified price-to-book:

```text
Justified P/B = (ROE - g) / (COE - g)
```

Where:

| Input | Assumption |
| --- | --- |
| Normalized ROE | ~17% |
| Long-term growth rate, `g` | ~4% |
| Risk-free rate | ~4.3% |
| Beta | ~1.0 |
| Equity risk premium | ~4.8% |
| Cost of equity, `COE` | ~9.1% |

The intuition is simple: a bank that earns a higher ROE than its cost of equity should be worth more than book value. With JPM, the model produces a justified P/B of about 2.5x. Applied to book value per share of about $127, that gives a target price of about $324.

The model also checks the ROE implied by the current price. At a market price of about $334, the implied ROE is about 17.4%, almost exactly JPM's recent actual ROE. That suggests the market is already pricing JPM as if it can continue earning peak returns, which supports a Neutral / Hold rating rather than a Buy.

## Key FY2025 Figures

| Metric | FY2025 |
| --- | ---: |
| EPS | $20.02 |
| BVPS | $126.99 |
| ROE | 17.0% |
| ROTCE | 20.0% |
| CET1 ratio | 14.6% |
| Efficiency ratio | ~52% |

## Files

- [Model workbook](model/JPM_Model_Lite.xlsx)
- [Research note](research-note/JPM_Research_Note.pdf)
- [Bank concepts](docs/CONCEPTS.md)
- [Valuation methodology](docs/METHODOLOGY.md)

## What I Learned / Caveats

This project reinforced that bank valuation is mostly about the relationship between returns, capital, and book value. JPMorgan can deserve a premium multiple because it earns well above its cost of equity, but a premium business is not automatically a mispriced stock.

Income-statement figures are from JPM's FY2022 and FY2025 Annual Reports and quarterly releases; NII is on a managed basis. Some per-share and balance-sheet items are summary figures and should be reconciled to the 10-K before quoting. All assumptions are illustrative and my own. This is a self-directed analytical exercise, not investment advice, and it contains no non-public information.
