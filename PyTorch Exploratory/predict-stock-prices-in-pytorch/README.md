# Predict Stock Prices with LSTM in PyTorch

This project demonstrates how to build and evaluate a Long Short-Term Memory (LSTM) neural network using PyTorch to predict stock closing prices based on daily Open, High, Low, and Close values.

## Overview

The notebook walks through the following steps:
- **Data Loading & Preparation:**  
  Loads historical stock price data, sorts it chronologically, and selects relevant features.
- **Data Normalization:**  
  Scales the features to a uniform range using MinMaxScaler.
- **Sequence Creation:**  
  Prepares input/output sequences for time series forecasting.
- **Model Definition:**  
  Implements an LSTM model in PyTorch for regression.
- **Training:**  
  Trains the model to predict the next day's closing price.
- **Evaluation:**  
  Converts predictions back to original scale and evaluates performance using MAE and RMSE.
- **Visualization:**  
  Plots actual vs. predicted prices and their differences.

## Key Features

- **LSTM Model:**  
  Utilizes PyTorch's LSTM layer for time series prediction.
- **Custom Sequence Generation:**  
  Flexible function to create training and test sequences.
- **Performance Metrics:**  
  Calculates Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
- **Visualization:**  
  Matplotlib plots for easy comparison of actual and predicted values.

## Usage

1. **Install dependencies:**
    ```bash
    pip install torch pandas matplotlib scikit-learn
    ```

2. **Run the notebook:**  
   Open `notebook.ipynb` in Jupyter or VS Code and execute the cells step by step.

## File Structure

- `notebook.ipynb` — Main notebook with code, explanations, and results.
- `README.md` — Project overview and instructions.

## References

- [IBM Developer: Build a recurrent neural network using PyTorch](https://developer.ibm.com/tutorials/build-a-recurrent-neural-network-pytorch/?mhsrc=ibmsearch_a&mhq=#learning-objectives0)
- [Kaggle: Gold Stock Prices Dataset](https://kaggle.com/datasets/sahilwagh/gold-stock-prices)

---

**Author:** Adapted from IBM Developer tutorial  
**License:** For educational use