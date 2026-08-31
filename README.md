# Mutual Fund Manager Performance

This repository contains a regression-based analysis of mutual-fund manager
performance. The Jupyter notebook includes the Python code and saved outputs,
so the results can be viewed directly on GitHub without rerunning the analysis.

## Analysis included

- Original and streamlined OLS models
- Model-specification and heteroskedasticity tests
- Candidate return predictions
- One-sided hypothesis tests
- Robust standard errors and confidence intervals
- Fund-type comparison and Welch t-test
- Individual-fund and diversified-portfolio predictions
- Manager-age analysis

## Files

- `mutual_fund_manager_performance.ipynb` — complete code, explanations, tables,
  statistical results, and diagnostic plots
- `requirements.txt` — Python packages needed to rerun the notebook

## Data

The licensed classroom case and its Excel dataset are not included. Authorized
users can place `case 3.xlsx` or `case 3.xls` in the notebook folder before
running the notebook.

## Run locally

```bash
pip install -r requirements.txt
jupyter notebook mutual_fund_manager_performance.ipynb
```
