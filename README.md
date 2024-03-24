# Project Overview

This project consists of five main folders, each containing different components and functionalities related to carbon intensity prediction and renewable energy forecasting.

## 1. Datasets

The `Datasets` folder contains three datasets:

- **Generated_datasets_for_Regressor_Model**: This dataset includes Mean Squared Error (MSE) data obtained after training various datasets using LSTM models. The datasets originate from the `Time_Series_Datasets` folder and encompass carbon intensity and percentage renewable energy data.

- **Generated_time_series_data**: Time series data acquired from the Tsfresh library. This data pertains to carbon intensity and percentage renewable energy.

- **Time_Series_Datasets**: Time series datasets for carbon intensity and percentage renewable energy.

## 2. Proposed Approach

The `Proposed_Approach` folder encompasses the proposed approach for carbon intensity prediction and renewable energy forecasting. It includes:

- Trained Random Forest Model
- Code for obtaining time series data using the `calculate_and_save_features` function from the `Tsfresh_data_extraction` folder.
- Combination of time series data with different hyperparameter combinations (Sequence Length and Scaler Type)
- Pretrained Random Forest model for predicting MSE
- Selection of optimal hyperparameters based on the least MSE

## 3. Regression Models

The `Regression_Models` folder contains three Python files:

- **data_preprocessing.py**: Prepares datasets from `Generated_datasets_for_Regressor_Model` and `Generated_time_series_data` for training and predicting MSE.
- **Testing_on_percentage_renewable_data.ipynb**: Uses carbon intensity data for training and renewable energy data for testing.
- **Testing_with_wholedata.py**: Utilizes all available datasets for training and testing. It also obtains the `random_forest_model.pkl` file.

## 4. Standard Approach

The `Standard_Approach` folder entails the training of an LSTM model using various hyperparameter combinations (Sequence Length and Scaler Type). It compares the results to determine the best hyperparameter combination.

## 5. Tsfresh Data Extraction

The `Tsfresh_data_extraction` folder contains the time series data extraction function, which utilizes the Tsfresh library.

