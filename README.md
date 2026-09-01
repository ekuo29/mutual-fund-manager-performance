# Mutual Fund Manager Performance Analysis

Regression analysis of 540 mutual-fund observations examining whether fund
type, undergraduate education, MBA status, manager age, and fund tenure help
explain excess returns. The project uses Python to evaluate model assumptions,
test the case hypotheses, compare candidate managers, and develop a hiring
recommendation.

## What the analysis covers

- Original and streamlined OLS return models
- Ramsey RESET, Breusch-Pagan, and White specification tests
- HC1 heteroskedasticity-robust inference
- Bob-versus-Putney return predictions
- One-sided coefficient tests and confidence intervals
- Growth versus growth-and-income fund comparisons
- Welch unequal-variance t-test
- Individual-fund and diversified-portfolio predictions
- Manager-age differences by fund type and MBA status

## Main findings

- The original model has a low R-squared, but the coefficients still provide
  useful evidence about systematic relationships in fund performance.
- Growth funds earned higher average excess returns than growth-and-income
  funds, and the equal-variance assumption was rejected.
- Putney's predicted excess return is 1.821 percentage points above Bob's if
  either candidate is hired to manage the new fund.
- A new Princeton-managed growth fund has an estimated excess return of 2.370%,
  although its individual prediction interval is wide.
- Growth-and-income managers are estimated to be 1.424 years older, holding
  educational background and fund tenure constant.
- Otherwise comparable MBA managers are estimated to be 1.879 years younger.

See the [case analysis](case_analysis.pdf) for the complete written discussion
and the [Jupyter notebook](mutual_fund_manager_performance.ipynb) for the Python
code, saved statistical output, and diagnostic plots.

## Repository files

```text
README.md                                Project overview
case_analysis.pdf                        Final written case analysis
mutual_fund_manager_performance.ipynb    Python code and saved output
case 3.xls                               Source data used by the notebook
requirements.txt                         Python dependencies
```

## Reproduce the Python analysis

Python 3.11 or newer is recommended.

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
jupyter notebook mutual_fund_manager_performance.ipynb
```

Keep `case 3.xls` in the repository folder, open the notebook, and run all cells
from the beginning.

## Publication and licensing

This repository contains the author's analysis. The assigned case and
instructions are not reproduced. The source workbook may be subject to
third-party classroom or publisher restrictions; confirm permission before
redistributing or reusing it outside the course context.

No open-source license has been applied. This repository does not grant
redistribution rights for the underlying case materials or data.
