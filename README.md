#  Stock Price Prediction using LSTM (TensorFlow)

## Project Overview

This project focuses on predicting stock prices using deep learning techniques, specifically Long Short-Term Memory (LSTM) networks. The model is trained on historical multi-stock market data and enhanced with technical indicators and engineered features to improve predictive performance.

The goal is to analyze time-series patterns and forecast future closing prices using machine learning.

---

## Problem Statement

Stock markets are highly volatile and influenced by complex patterns. This project aims to:

* Analyze historical stock data
* Engineer meaningful financial indicators
* Build an LSTM-based model for price prediction
* Evaluate model performance using regression metrics

---

## Dataset

* **Size:** 619,040 rows × 7 columns
* **Features:**

  * Date
  * Open
  * High
  * Low
  * Close
  * Volume
  * Stock Name (Ticker)
* Multi-company dataset covering several years of stock market data.

---

## Feature Engineering

To improve model performance, additional features were created:

* Moving Averages (MA20, MA50)
* Relative Strength Index (RSI)
* MACD (Moving Average Convergence Divergence)
* Signal Line
* Volume analysis

---

## Model Architecture

The model is built using TensorFlow/Keras:

* LSTM (64 units, return sequences)
* LSTM (64 units)
* Dense (32 units)
* Dropout (0.5)
* Output layer (1 unit)

Loss Function: Mean Squared Error (MSE)
Optimizer: Adam

---

## Training Process

* Sequence length: 60 time steps
* Epochs: 10–20
* Data normalization: MinMaxScaler (0–1 range)
* Train-test split: 95% training / 5% testing

---

## Evaluation Metrics

* **MSE:** 25.93
* **RMSE:** 5.09

The model shows moderate predictive performance, capturing general trends but struggling with short-term volatility.

---

## Key Insights

* The model learns temporal patterns effectively
* Feature engineering improves context but also introduces noise
* Stock prediction remains a highly challenging task due to market randomness
* Simpler feature sets may sometimes perform better than overly complex ones

---

## Future Improvements

* Train separate models per stock ticker
* Predict price movement (classification) instead of exact price
* Add sentiment analysis from financial news
* Experiment with GRU or Transformer-based models
* Optimize feature selection for reduced noise

---

## Tech Stack

* Python
* TensorFlow / Keras
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

##  Author

**Peter Njeri**
Mechanical Engineer | Machine Learning Engineer
GitHub: https://github.com/Kanjerih
LinkedIn: [www.linkedin.com/in/kanjerih](http://www.linkedin.com/in/kanjerih)
