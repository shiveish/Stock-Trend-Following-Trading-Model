# Stock Trend Following Trading Model

## Overview

This project implements a regression-based stock trading workflow using market index data and evaluates the resulting trading strategy on SPY price movements.

The project consists of three stages:

1. Simple linear regression modeling.
2. Multiple linear regression modeling using market indices.
3. Evaluation of a trading strategy derived from regression predictions.

---

## Repository Structure

```text
Stock-Trend-Following-Trading-Model/
│
├── simple_regression.py
├── multiple_regression.py
├── strategy_evaluation.py
│
├── Simple linear regression model.ipynb
├── Multiple linear regression model.ipynb
├── Evaluating strategy built from Regression model.ipynb
│
└── README.md
```

---

## Components

### 1. Simple Linear Regression Model

This module performs linear regression analysis and compares manually selected model parameters with fitted regression coefficients obtained through ordinary least squares estimation.

Implemented in:

* `Simple linear regression model.py`
* `Simple linear regression model.ipynb`

---

### 2. Multiple Linear Regression Model

This module builds a multiple linear regression model using lagged market information and global equity indices as explanatory variables.

The implemented predictors include:

* SPY lagged return
* S&P 500
* NASDAQ
* Dow Jones Industrial Average
* CAC 40
* DAX
* Nikkei
* Hang Seng Index
* All Ordinaries Index

Implemented in:

* `Multiple linear regression model.py`
* `Multiple linear regression model.ipynb`

---

### 3. Trading Strategy Evaluation

This module converts regression predictions into trading positions and evaluates strategy performance.

The implementation includes:

* Trading signal generation
* Strategy return calculation
* Cumulative return analysis
* Sharpe ratio calculation
* Maximum drawdown calculation
* Benchmark comparison

Implemented in:

* `Evaluating strategy built from Regression model.py`
* `Evaluating strategy built from Regression model.ipynb`

---

## Dependencies

The project uses the following Python libraries:

* numpy
* pandas
* matplotlib
* statsmodels

---

## Running the Project

Execute the Python scripts individually or run the corresponding Jupyter notebooks.

Example:

```bash
python "Multiple linear regression model.py"
```
