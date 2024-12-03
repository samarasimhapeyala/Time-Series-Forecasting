# 📈 Time-Series Forecasting

Stock Price forecasting using time series techniques and LSTM.

# 📁 Project Structure

This repository contains the following folders:
   
## 1. 📈 Stock Market Prediction and Forecasting Using Stacked LSTM

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

## 2. 📈 Univariate Time Series Forecasting Using LSTM

This project demonstrates how to use Long Short-Term Memory (LSTM) networks to perform univariate time series forecasting. The focus is on predicting future values based on a single variable's historical data.

---

## 🗂 Overview

### 📊 Data
- A simple univariate time series dataset is used: `[110, 125, 133, 146, 158, 172, 187, 196, 210]`.
- The sequence is split into sliding windows of input (`X`) and target (`y`) values, with each sample containing 3 timesteps.

### 🧠 Model
- **LSTM Architecture**:
  - Two stacked LSTM layers with 50 units each, using ReLU activation.
  - One Dense layer with 1 neuron for the output.
  - The model is compiled with the **Adam optimizer** and **Mean Squared Error (MSE)** as the loss function.
- The model is trained for **300 epochs** on the prepared dataset.

### 📈 Prediction
- After training, the model predicts the next 10 values in the series using a loop-based approach:
  - Each prediction is fed back into the input to generate subsequent forecasts.
  - The predicted values extend the time series into the future.

### 📉 Visualization
- The original time series and the predicted future values are visualized using matplotlib.
- This allows for a clear comparison between the known data and the forecasted values.

---

## 🔍 Results
- The model successfully forecasts the next 10 values in the series.
- Predictions demonstrate the LSTM's ability to learn and extend patterns in the time series.

---

## 📋 How to Use
1. Prepare your univariate time series data.
2. Adjust the number of timesteps (`n_steps`) as required for your use case.
3. Train the LSTM model using the provided architecture.
4. Use the trained model to predict future values iteratively.
5. Visualize the results for validation.

---

This project is a great starting point for building advanced time series forecasting models tailored to real-world datasets.


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
