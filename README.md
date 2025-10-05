# Stock Price Prediction using Stacked LSTM

## Overview
This project is an implementation of a stock price prediction model using a stacked Long Short-Term Memory (LSTM) network. The model is built using TensorFlow and Keras and is designed to forecast future stock closing prices based on historical data from the last five years.The model fetches live historical data, preprocesses it, trains the LSTM network, and finally, predicts the stock price for the next 30 days.

The methodology is based on the concepts demonstrated in a tutorial by **Krish Naik**. 

## Features
- **Data Collection**: Fetches 5 years of historical stock data for any ticker using the `yfinance` library.
- **Data Preprocessing**: Scales the closing price data using `MinMaxScaler` to prepare it for the LSTM model.
- **Model Architecture**: Implements a stacked LSTM network with three LSTM layers and a final Dense layer for output.
- **Training & Evaluation**: Trains the model on 70% of the historical data and validates it on the remaining 30%.
- **Prediction Visualization**: Plots the model's predictions on the training and test data with  the original stock prices.
- **Future Forecasting**: Predicts the stock price for the next 30 days based on the last 100 days of available data and visualizes the forecast.
