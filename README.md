# Bitcoin Price Prediction - Summary README

## Overview

This project focuses on predicting Bitcoin prices against USD using a combination of time series and machine learning models. The project aims to provide valuable insights for traders and investors by leveraging historical price data.

## Key Features

- **Data Source:** The dataset is sourced from [investing.com](https://investing.com/), spanning from July 18, 2010, to the present day. It includes daily Bitcoin vs USD exchange rates, opening/closing prices, high/low prices, trading volume, and daily percentage changes.

- **Business Objective:** Develop a robust model capable of accurately forecasting daily Bitcoin prices to assist traders and investors in making informed decisions.

## Project Structure

### 1. Exploratory Data Analysis (EDA)

- **Data Understanding:** Load and inspect the dataset, exploring key metrics.
- **Data Cleaning:** Handle missing values, duplicates, and check data types.
- **Exploratory Data Analysis (EDA):** Visualize closing prices and daily returns over time.
- **Feature Engineering:** Create additional relevant features, such as daily returns.

### 2. Model Development

#### Time Series Models

- **ARIMA (AutoRegressive Integrated Moving Average):** Utilize the SARIMAX model to predict Bitcoin prices. The optimal order is determined using the auto_arima function.

#### Machine Learning Models

- **LSTM (Long Short-Term Memory):** Implement a deep learning model for prediction. Data is preprocessed using MinMax scaling, and the dataset is split into training and testing sets.

- **Facebook Prophet Model:** Utilize the Prophet model for forecasting univariate time series data. Evaluate and compare the performance with other models.

#### Vector Autoregressive (VAR) Model

- Use VAR to model the interdependence between price, volume, and change features.

### 3. Model Evaluation

- Assess the performance of each model using appropriate metrics.
- Compare the accuracy of time series models, machine learning models, and the VAR model.

### 4. Model Deployment

- Deploy the Facebook Prophet model for real-time data extraction and forecasting.
- Create a Streamlit web app for users to interact with the deployed model.

## Results

- The project evaluates the effectiveness of various models in predicting Bitcoin prices, considering both univariate and multivariate approaches.
- The Facebook Prophet model on 1-lag differenced series outperforms other models, achieving an RMSE of 855.996.

## Contributors

- **Leonard Gachimu**
- **Francis Njenga**
- **Thomas Okiwi** 

## Acknowledgments

- Special thanks to [investing.com](https://investing.com/) for providing the dataset.
- This project is inspired by the dynamic nature of cryptocurrency trading and the need for accurate price predictions.

## License

This project is licensed under the [MIT License](LICENSE).

Feel free to contribute, raise issues, or use the code for your own analysis!
