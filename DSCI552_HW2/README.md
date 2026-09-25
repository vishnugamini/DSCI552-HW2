# DSCI 552 - Homework 2

Vishnu Gamini · GitHub: vishnugamini

Regression analysis of the Combined Cycle Power Plant dataset and solutions to ISLR exercises 2.4.1 and 2.4.7.

## Files

```text
data/CCPP/Folds5x2_pp.xlsx
notebook/Gamini_Vishnu_HW2.ipynb
requirements.txt
```

## Run locally

Use Python 3.12. From the repository root:

```sh
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m notebook
```

Open `notebook/Gamini_Vishnu_HW2.ipynb`, choose the environment's Python kernel, and run all cells. The notebook includes saved outputs and reads the bundled workbook using a relative path. Only Sheet1 is analyzed.

The prediction comparisons use a 70/30 split with random seed 42. Normalization and variable selection are fitted on training data. Regression significance tests use a 5% threshold; backward elimination preserves main effects required by higher-order terms.

## Dataset

Tüfekci, P., and Kaya, H. (2014). *Combined Cycle Power Plant*. UCI Machine Learning Repository. https://doi.org/10.24432/C5002N.

