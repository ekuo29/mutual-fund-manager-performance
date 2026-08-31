# Mutual Fund Manager Performance

This project uses regression analysis to examine whether fund type, education,
age, and fund tenure help explain mutual-fund excess returns.

## View the completed analysis

Open [`mutual_fund_manager_performance.ipynb`](mutual_fund_manager_performance.ipynb)
to view the Python code together with the saved regression tables, statistical
tests, predictions, conclusions, and diagnostic plots. The notebook can be
viewed directly on GitHub without rerunning it.

## Methods

- Original and streamlined OLS regressions
- Ramsey RESET, Breusch-Pagan, and White tests
- HC1 heteroskedasticity-robust inference
- One-sided hypothesis tests and confidence intervals
- Welch unequal-variance t-test
- Individual-fund and diversified-portfolio predictions

## Selected results

- Growth funds have higher average excess returns than growth-and-income funds.
- Putney's model-predicted excess return is 1.821 percentage points above Bob's
  if either candidate is hired to manage the new fund.
- Growth-and-income managers are estimated to be 1.424 years older, holding
  education and tenure constant.
- Otherwise comparable MBA managers are estimated to be 1.879 years younger.

## Repository files

- `mutual_fund_manager_performance.ipynb` — complete analysis with saved output
- `case 3.xls` — data used by the notebook
- `requirements.txt` — required Python packages

## Run locally

```bash
pip install -r requirements.txt
jupyter notebook mutual_fund_manager_performance.ipynb
```

## Data note

The Excel file originates from licensed classroom material. Confirm that you
have permission before redistributing or reusing it outside the course context.
