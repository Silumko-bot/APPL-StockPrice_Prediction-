# Overview
This project demonstrates an end-to-end approach to forecasting Apple Inc. (AAPL) closing stock prices by combining classical and deep learning techniques. The hybrid model leverages both Linear Regression and a Long Short-Term Memory (LSTM) neural network to capture linear trends and complex nonlinear patterns in historical stock data. The goal is to provide robust, accurate short-term price predictions for use in financial analysis and trading strategies.

# Objective
Develop a hybrid machine learning model that accurately predicts Apple’s daily closing stock price by integrating Linear Regression (for linear trends) and LSTM (for nonlinear residuals). Evaluate the model’s predictive performance and visualize its effectiveness, providing actionable insights for investors and analysts.

# Motivation
Stock price prediction is a critical task in quantitative finance, with direct applications in trading, risk management, and investment decision-making. Traditional models often struggle to capture the complex, nonlinear behavior of financial time series. This project explores whether a hybrid approach can deliver superior accuracy and reliability, making it a valuable tool for real-world financial forecasting.

# Data
Source: Historical daily price data for Apple Inc. (AAPL)

Features: Date, Open, High, Low, Close, Volume

Engineered Features: Lagged closing prices (close_lag1, close_lag2, close_lag3) to capture short-term dependencies

# Methodology

Data Preparation

Loaded and cleaned historical price data

Engineered lagged features for time series modeling

Scaled features and target variable for model compatibility

Modeling Approach

Linear Regression: Modeled the primary linear trends in the closing price

LSTM Neural Network: Trained on the residuals (errors) from the linear model to capture nonlinear patterns

Hybrid Model: Combined predictions from both models for final forecasts

Evaluation

Assessed model performance using RMSE, MAE, and MAPE

Visualized actual vs. predicted closing prices over the test period

# Findings
The hybrid model achieved strong predictive accuracy, with the following metrics on the test set:

RMSE: 1.23

MAE: 1.01

MAPE: 3.45%

As shown in the figure below, the hybrid model’s predictions (orange dashed line) closely track the actual closing prices (blue line), even during periods of volatility and trend shifts.

The model effectively captures both long-term trends and short-term fluctuations, demonstrating the value of combining classical and deep learning approaches for financial forecasting.

# Conclusion

This project demonstrates that a hybrid machine learning approach can deliver robust and accurate short-term forecasts for Apple’s stock price. The combination of Linear Regression and LSTM enables the model to capture both linear and nonlinear dynamics in the data, outperforming standalone models. This methodology is adaptable to other stocks and financial time series, offering significant potential for real-world trading and investment strategies.

# How to Use
Clone the repository and install required dependencies (see requirements.txt).

Run the Jupyter notebook to reproduce the analysis, modeling, and visualizations.

Adjust the code to apply the hybrid modeling approach to other stocks or time series datasets.

Future Work
Incorporate additional features such as technical indicators, macroeconomic data, or news sentiment

Experiment with alternative neural network architectures (e.g., GRU, Transformer)

Extend the approach to multi-step and long-term forecasting

Author
Silumko Mbetha 
Data Scientist | Financial Modeling Enthusiast

For questions or collaboration opportunities, please contact me via Email:sdmbetha2@gmail.com or [LinkedIn]](https://www.linkedin.com/in/silumko-mbetha-98931b2b8/).







