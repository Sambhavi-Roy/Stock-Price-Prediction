# Stock Price Prediction

This project aims to predict stock prices using various machine learning models including Linear Regression, Support Vector Regression (SVR), and Random Forest Regressor. The dataset used contains historical stock prices of HINDUNILVR.NS.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)


## Introduction

Predicting stock prices is a challenging task due to the volatile nature of financial markets. This project implements multiple regression models to predict the closing prices of a stock based on historical data.


## Features

- Data preprocessing including date format conversion
- Implementation of multiple regression models:
  - Linear Regression
  - Support Vector Regression (SVR)
  - Random Forest Regressor
- Evaluation of models using Mean Squared Error (MSE)
- Prediction of future stock prices


## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Sambhavi-Roy/Stock-Price-Prediction.git

2. Navigate to the project directory:
   '''bash
  cd stock-price-prediction

3. Install the required packages:
  '''bash
  pip install numpy pandas scikit-learn


## Usage

1. Load the dataset:
  Ensure the HINDUNILVR.NS.csv file is placed in the project directory or provide the correct path to the file.

2. Run the script:
  '''bash
  python stock_prediction.py

3. The script will:
  - Load and preprocess the data
  - Split the data into training and testing sets
  - Train and evaluate multiple regression models
  - Output evaluation metrics and predicted stock prices for future dates


## Results

- Linear Regression:
  Training MSE: 7208.711195733958
  Validation MSE: 11596.274163636783
  
- Support Vector Regression (SVR):
  Training MSE: 2.0018210112496108e+16
  Validation MSE: 2.0028674246510212e+16
  
- Random Forest Regressor:
  Training MSE: 167.12545276674126
  Validation MSE: 557.8318999397642


- Example Prediction
  To predict the stock price for a specific future date, update the future_date variable in the script and run the predictions:
  
  future_date = np.array([20240607]).reshape(-1, 1)  # Change the date accordingly
  predicted_price = model.predict(future_date)
  print("Predicted Stock Price:", predicted_price[0])


## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
