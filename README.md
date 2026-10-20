# Drivers of the Nikkei 225

Econometrics project, MSc Data & Corporate Finance (Audencia, Paris).

**Question:** which macro and market variables explain the monthly moves of the Nikkei 225, and how much?

## Approach

1. **Data**: monthly series for the index and candidate drivers (FX, rates, global equities, macro indicators), cleaned and aligned on a common calendar
2. **Model**: OLS regression on monthly returns, estimated in Python (`statsmodels`) and cross-checked in Excel
3. **Diagnostics**: significance, multicollinearity, residual checks, robustness
4. **Story**: results turned into a 10 minute presentation for a non-specialist audience

## Stack

`Python` `Pandas` `statsmodels` `Excel`

## Status

🚧 In progress. Notebook, data pipeline and final results will be added as the project moves forward.
