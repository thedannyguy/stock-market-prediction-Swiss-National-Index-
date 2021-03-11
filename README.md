# Stock-Market-Prediction-Swiss-National-Index-

Note: my blog post can be viewed at https://thedannyguy.medium.com/predicting-stock-market-price-movement-in-switzerland-60e23c0ddcd4

# Description
This project is about stock market prediction (Swiss Market Index) and has 4 steps:
1) First we will gather the necessary fundamental features from Yahoo and Investing API and technical features from pandas_tA module. We are required to perform re-indexing and linear interpolation to fill missing values. We then convert the closing prices of Swiss Market Index to 1, 3 and 5-day returns.
2) To answer our first research question, we will use Chi-squared and mutual information classification to identify the 10 most important features for 1, 3 and 5-day forecast horizon.
3) To answer our second research question, we will use Pearson correlation coefficient to determine features that are positively and negatively related to returns.
4) To answer our final research question, we will use XGBoost model and train our model using Bayesian optimisation. We would select the top 3 best hyperparameter combinations for each forecast horizon and calculate the mean accuracy and F1 score.

# Dependencies
This repository is written in Python and the following Python packages are required: numpy, pandas, investpy, yfinance, pandas_datareader, pandas_ta, sklearn.ensemble, sklearn.feature_selection, matplotlib.pyplot, scipy and sklearn.preprocessing

# File description
Udacity Project Workbook 1.ipynb : notebook containing all the codes for this project

all_fundamental indicators.csv : csv file containing all the fundamental variables

all_technical_indicators.csv: csv file containing all the technical variables

all_indicators_with_forecast_return.csv: csv file containing all the fundamental and technical variables and the target variables of 1, 3 and 5-day return

Screenshots: screenshots of bar graphs that are used to answer the research questions.

# Outcome
1. I managed to idenfify the 10 most important features for 1, 3 and 5-day forecast horizons.
2. I managed to identify features that are positively and negatively related to my target variables of 1, 3 and 5-day return.
3. I managed to identify the forecast horizon that produces the highest mean accuracy and F1 scores. (namely 1-day horizon)
