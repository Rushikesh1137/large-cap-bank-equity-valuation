# Valuation Methodology

This project values JPMorgan Chase using a justified price-to-book framework. The model does not use enterprise value or EV/EBITDA because those are not clean valuation tools for banks.

## Step 1: Start With Bank-Appropriate Valuation

Banks are valued directly on equity. Deposits and borrowings are not just financing; they are raw material for the lending business. Because of that, the key question is whether the bank earns enough return on its equity capital to justify trading above book value.

## Step 2: Use Justified Price-to-Book

The core relationship is:

```text
Justified P/B = (ROE - g) / (COE - g)
```

Where:

- `ROE` is the normalized return on equity.
- `g` is the long-term growth rate.
- `COE` is the cost of equity.

The intuition is that a bank earning a higher ROE than its cost of equity is worth more than book value. Strong banks trade above book because they compound equity at attractive returns. Weak banks can trade near or below book when returns are poor.

## Step 3: Estimate Cost of Equity

The model estimates cost of equity using CAPM:

```text
COE = risk-free rate + beta x equity risk premium
```

The assumptions are:

| Input | Assumption |
| --- | ---: |
| Risk-free rate | ~4.3% |
| Beta | ~1.0 |
| Equity risk premium | ~4.8% |
| Cost of equity | ~9.1% |

## Step 4: Apply JPMorgan Assumptions

The key operating assumption is normalized ROE of about 17%, which is close to JPMorgan's recent reported ROE. The long-term growth assumption is about 4%.

| Input | Assumption |
| --- | ---: |
| Normalized ROE | ~17% |
| Long-term growth rate | ~4% |
| Cost of equity | ~9.1% |

Using the justified P/B formula, these assumptions support a justified P/B multiple of about 2.5x.

## Step 5: Convert Multiple to Target Price

The target price is:

```text
Target price = justified P/B x book value per share
```

Using about 2.5x book value and book value per share of about $127, the model produces a target price of about $324.

## Step 6: Reality-Check With Market-Implied ROE

The model also rearranges the justified P/B formula to solve for the ROE implied by the current market price. At a price of about $334, the implied ROE is about 17.4%.

That is very close to JPMorgan's actual recent ROE. The conclusion is that the market already expects JPMorgan to keep earning very strong returns. That leaves limited margin of safety even though the company is high quality.

## Conclusion

The valuation conclusion is:

| Item | Result |
| --- | --- |
| Rating | Neutral / Hold |
| Target price | ~$324 |
| Market price | ~$334 |
| Implied upside / downside | ~3% downside |

JPMorgan appears to be the best-run large-cap US bank, with FY2025 ROE of about 17%, ROTCE of about 20%, CET1 of about 14.6%, and an efficiency ratio around 52%. The issue is valuation: at roughly 2.6x book and 16.7x earnings, much of that quality is already reflected in the price.
