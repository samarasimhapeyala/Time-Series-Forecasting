# 📈 Time-Series Forecasting

Stock Price forecasting using time series techniques and LSTM.

## 📁 Project Structure

This repository contains the following folders:

1. **Stock Market Forecasting**  
   Techniques and methods for stock market price prediction.
# 📈 Stock Market Prediction and Forecasting Using Stacked LSTM

This project predicts and forecasts stock prices using Stacked Long Short-Term Memory (LSTM) networks, a type of recurrent neural network (RNN) well-suited for time-series data.

## 🗂 Overview

### 📊 Data
- Historical stock data (e.g., Apple stock) is used for training and testing the model.
- Data includes features such as `Open`, `High`, `Low`, `Close`, and `Volume`.
- The data is normalized using `MinMaxScaler` to improve model performance.

### 🧠 Model and Algorithm
- **Stacked LSTM**: 
  - Three LSTM layers with 50 units each.
  - One Dense layer with a single neuron for output.
  - The model is compiled using the **Adam optimizer** and trained to minimize **Mean Squared Error (MSE)**.

- **Key Features**:
  - Sliding window approach to create sequences for training.
  - Time-series data split into 70% training and 30% testing.

### 📈 Evaluation
- Root Mean Squared Error (RMSE) is calculated for both training and testing predictions:
  - **Training RMSE**: 182.70
  - **Testing RMSE**: 24.00

### 📉 Visualization
- The model predictions are compared with actual stock prices using matplotlib.
- Results demonstrate the model's ability to capture trends and fluctuations in stock prices.

## 🔍 Conclusion
This project successfully applies Stacked LSTMs to predict stock prices with good accuracy, providing a strong foundation for future time-series forecasting tasks.


3. **Univariate Time Series Forecasting**  
   Implementation of forecasting for single-variable time series data.

## 💡 About

This project aims to forecast stock prices by leveraging time-series analysis methods such as:

- Traditional statistical models
- Machine learning approaches
- Long Short-Term Memory (LSTM) neural networks

## 🚀 Features

- Implementation of statistical models like ARIMA and SARIMA
- Machine Learning-based time-series forecasting
- Deep learning methods with LSTM for improved accuracy


Feel free to fork and contribute to this project! 😊
