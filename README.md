# Project Overview

This project consists of five main folders, each containing different components and functionalities. The primary objective is to forecast the most effective hyperparameters for time series datasets prior to actual training. By doing so, the project contributes to advancements in sustainability and energy efficiency. The project employs LSTM (Long Short-Term Memory) time series models to achieve its goals.

## 1. Datasets

The `Datasets` folder contains three datasets:

- **Generated_datasets_for_Regressor_Model**: This dataset includes Mean Squared Error (MSE) data obtained after training various datasets using LSTM models. The datasets used for training are carbon intensity and percentage renewable energy data which are uploaded in the `Time_Series_Datasets` folder.

- **Generated_time_series_data**: Time series data acquired from the Tsfresh library. This data pertains to carbon intensity and percentage renewable energy.

- **Time_Series_Datasets**: Time series datasets for carbon intensity and percentage renewable energy.

## 2. Proposed Approach

The `Proposed_Approach` folder encompasses the proposed approach for carbon intensity prediction and renewable energy forecasting. The steps of the proposed approach are:

- Time series data using the `calculate_and_save_features` function from the `Tsfresh_data_extraction` folder is obtained.
- Extracted time series data along with different hyperparameter combinations (Sequence Length and Scaler Type) is given as input to the pretrained Random Forest model for predicting MSE.
- Selection of optimal hyperparameters based on the least MSE

## 3. Regression Models

The `Regression_Models` folder contains three Python files:

- **data_preprocessing.py**: Prepares datasets from `Generated_datasets_for_Regressor_Model` and `Generated_time_series_data` for training and predicting MSE.
- **Testing_on_percentage_renewable_data.ipynb**: Uses random forest regressor on carbon intensity data for training and testing is done on renewable energy data.
- **Testing_with_wholedata.py**: Utilizes all available datasets for training and testing. This file obtaines `random_forest_model.pkl` file.

## 4. Standard Approach

The `Standard_Approach` folder entails the training of an LSTM model using various hyperparameter combinations (Sequence Length and Scaler Type). It compares the results to determine the best hyperparameter combination.

## 5. Tsfresh Data Extraction

The `Tsfresh_data_extraction` folder contains the time series data extraction function, which utilizes the Tsfresh library.

