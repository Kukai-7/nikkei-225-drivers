# Who moves the Nikkei? Drivers of Japanese equity returns, 2005 to 2026

Group project, *Statistics & Econometrics*, MSc Data & Corporate Finance (Audencia).

**Question:** to what extent do external macro-financial factors (the yen, US equities, oil, the US-Japan rate gap) explain the monthly return of the Nikkei 225, do they still matter once Japan's own Fama-French factors are controlled for, and did the 2026 oil shock change the answer?

## Key results

| | Finding |
|---|---|
| **External drivers** | Yen (β 0.87) and S&P 500 (β 0.86) explain **64%** of monthly Nikkei returns. Oil and the rate gap add nothing before 2026 (joint F p = 0.28) |
| **2026 oil regime** | From March 2026 the oil beta flips from +0.02 to **−0.18** (interaction p < 0.001). Both Chow tests reject stability |
| **Abnormal returns** | March 2026 is the one month the model badly misses (−12.3 pp, t = −3.6); cumulatively the shock washes out (CAR +3.9%, t = 0.4) |
| **Japan factor model** | Final model FF5 − CMA + momentum: **adj. R² 0.91**, market β 1.08, large-cap growth tilt, no significant alpha |
| **Model selection** | Nested F-tests, likelihood-ratio tests, AIC and BIC all pick the same model |
| **Tails** | Returns are Student-t with about 6 degrees of freedom: the 2008 crash is a 1-in-2,000 month, not 1-in-3-million |

## What's inside

1. Descriptive statistics, normality and unit-root tests
2. OLS with Newey-West errors, VIF, Breusch-Pagan, Breusch-Godfrey, Durbin-Watson
3. Structural break: dummy, interaction, abnormal returns, predictive and classic Chow tests
4. CAPM, FF3, FF5 and Carhart-style models on Kenneth French's Japan factors
5. Expected excess return from factor premia (about 4.2% a year)
6. Maximum likelihood: MLE = OLS check, LR tests, AIC/BIC, Student-t fit, simulation of estimator precision
7. Limitations, stated up front

## Data

Monthly, December 2005 to September 2026. Market series from Yahoo Finance, factors from the Kenneth French Data Library. The notebook expects `dataset.csv` and `dataset_ff_japan.csv` in the same folder.

## Stack

`Python` `Pandas` `statsmodels` `SciPy` `Matplotlib`

## Limitations

Seven months of oil regime is a small sample, nothing here is causal, and the break date is a modelling choice. See the last section of the notebook.
