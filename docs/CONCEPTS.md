# Bank Valuation Concepts

This note defines the banking terms used in the JPMorgan valuation model and explains why a bank is valued differently from a normal operating company.

## Why Banks Are Different

For a normal company, debt is financing. Analysts often value the whole enterprise using discounted free cash flow or enterprise-value multiples, then subtract net debt to arrive at equity value.

For a bank, deposits and borrowings are raw material. They are the input the bank lends out to earn income. This makes enterprise value and free cash flow less meaningful for banks. Instead, bank valuation focuses directly on equity through methods such as price-to-book versus return on equity, residual income / justified P/B, and dividend or total-payout models.

## Core Banking Metrics

| Metric | Definition | Why it matters |
| --- | --- | --- |
| Net interest income (NII) | Interest earned on loans and securities minus interest paid on deposits and borrowings. | It is a bank's core spread income. |
| Net interest margin (NIM) | NII divided by average interest-earning assets. | It expresses the spread as a percentage. |
| Noninterest revenue | Fee income, including trading, investment banking, asset and wealth management, card, and payment fees. | It shows revenue that is not directly interest spread income. |
| Efficiency ratio | Noninterest expense divided by total revenue. | Lower is better because it signals cost discipline. Around 50%-55% is strong for a large bank. |
| Provision for credit losses / credit cost | Provision is the expense set aside for expected loan losses. Credit cost equals provision divided by average loans. | It captures the expected cost of credit risk. |
| Return on equity (ROE) | Net income to common shareholders divided by average common equity. | It is the headline profitability measure for a bank. |
| Return on tangible common equity (ROTCE) | Net income to common divided by average tangible common equity, excluding goodwill and intangibles. | Banks emphasize it because acquisitions create goodwill that can flatter book value. |
| Book value per share (BVPS) | Common equity divided by shares. | It is the per-share equity base used in price-to-book valuation. |
| Tangible book value per share (TBVPS) | Common equity excluding goodwill and intangibles, divided by shares. | It focuses on tangible shareholder equity. |
| CET1 ratio | Common Equity Tier 1 capital divided by risk-weighted assets. | It is the key regulatory measure of bank safety and solvency. Higher means more cushion. |

## Valuation Multiples

| Multiple | Formula |
| --- | --- |
| P/E | Price divided by EPS |
| P/B | Price divided by BVPS |
| P/TBV | Price divided by TBVPS |
| Dividend yield | Dividend per share divided by price |

These multiples are most useful when connected to the underlying economics of the bank. In this project, P/B is interpreted through ROE: a bank earning more than its cost of equity can justify trading above book value.
