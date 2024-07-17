# Stock Price Prediction

This repository contains a project aimed at predicting Tesla's stock prices using Linear Regression. The project involves preprocessing the data, feature engineering, splitting the dataset into training, testing, and validation sets, training a linear regression model, and visualizing the results.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [Contributing](#contributing)

## Overview

This project demonstrates a basic approach to predicting stock prices using machine learning. The goal is to forecast the closing prices of Tesla (TSLA) stocks based on historical data using a linear regression model.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/devanshisaraf/Stock-Price-Prediction.git
    cd Stock-Price-Prediction
    ```

2. Create and activate a virtual environment (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:

## Usage

1. Ensure you have the dataset file `TSLA.csv` in the root directory of the project.

2. Run the Jupyter notebook `Stock_Price_Prediction.ipynb` to see the full analysis and model training process. You can do this by launching Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

3. Open `Stock_Price_Prediction.ipynb` and execute the cells to run the analysis.

## Dataset

The dataset used in this project contains historical stock prices for Tesla. The main features include:
- Date
- Open
- High
- Low
- Close
- Volume

Make sure to download and place the dataset (`TSLA.csv`) in the root directory of the project.

## Model Training and Evaluation

The project follows these main steps:
1. **Data Preprocessing**: Handles missing values and converts the 'Date' column to datetime format.
2. **Feature Engineering**: Extracts new features such as year, month, and day, and uses the previous day's closing price as a feature.
3. **Splitting Data**: Divides the data into training, testing, and validation sets.
4. **Model Training**: Trains a linear regression model on the training set.
5. **Model Evaluation**: Evaluates the model using mean squared error (MSE) and R² score on the training, testing, and validation sets.
6. **Visualization**: Plots the actual vs. predicted closing prices and shows a correlation heatmap.

## Results

The model's performance is evaluated using the following metrics:
- **Train MSE**
- **Train R²**
- **Test MSE**
- **Test R²**
- **Validation MSE**
- **Validation R²**

Visualization includes:
- Correlation Heatmap
- Time Series Plot of Actual vs. Predicted Closing Prices

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any enhancements or bug fixes. 

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.
