# Gold Price Regression (Time Series Financial Modeling)

## Project Overview

This project predicts **Gold Closing Price** using macroeconomic and
financial indicators such as:

-   S&P 500 ETF (SP500)
-   Nasdaq ETF
-   US Interest Rates
-   CPI (Inflation)
-   Forex Rates (USD/CHF, EUR/USD)
-   GDP
-   Silver, Oil, Platinum, Palladium prices

The dataset combines daily market data with macroeconomic indicators,
making it a time series regression problem.

------------------------------------------------------------------------

## Problem Type

-   Supervised Learning
-   Regression
-   Time Series Forecasting (non-random split)

Target Variable: gold close

------------------------------------------------------------------------

## Project Structure

gold-price-regression/ │ ├── data/ │ └── financial_regression.csv │ ├──
notebooks/ │ └── exploration.ipynb │ ├── src/ │ └── train.py │ ├──
outputs/ │ └── model_results.txt │ ├── requirements.txt └── README.md

------------------------------------------------------------------------

## Machine Learning Workflow

1.  Load financial dataset
2.  Handle missing values using forward fill
3.  Remove remaining null values
4.  Separate features and target
5.  Perform time-based train-test split (80/20)
6.  Scale features
7.  Train Linear Regression model
8.  Evaluate using:
    -   Mean Squared Error (MSE)
    -   R² Score

------------------------------------------------------------------------

## Model Used

Linear Regression

Optional Upgrade: XGBoost Regressor for improved nonlinear performance

------------------------------------------------------------------------

## How To Run

1.  Install dependencies:

pip install -r requirements.txt

2.  Run training script:

python src/train.py

------------------------------------------------------------------------

## Evaluation Metrics

-   MSE (Mean Squared Error)
-   R² Score

------------------------------------------------------------------------

## Future Improvements

-   Add lag features for time-series modeling
-   Use XGBoost or LightGBM
-   Perform TimeSeriesSplit cross-validation
-   Feature importance analysis
-   Hyperparameter tuning

------------------------------------------------------------------------

## Author

Machine Learning project focused on financial time-series regression and
model evaluation.
