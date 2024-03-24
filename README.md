Project Overview
This project aims to optimize hyperparameters for renewable energy forecast models using carbon intensity and percentage renewable energy time series data. The project is structured into five main folders, each serving a specific purpose in the analysis and optimization process.

1. Datasets
The Datasets folder contains three subfolders:

Generated_datasets_for_Regressor_Model: This folder stores Mean Squared Error (MSE) data obtained after training LSTM models with different hyperparameter combinations. The hyperparameters include sequence length and scaler type. Data is generated for carbon intensity and percentage renewable energy datasets.

Generated_time_series_data: Time series data acquired from the Tsfresh library is stored here. The data includes time series features extracted from carbon intensity and percentage renewable energy datasets.

Time_Series_Datasets: This folder contains raw time series datasets for carbon intensity and percentage renewable energy.

2. Proposed Approach
The Proposed Approach folder includes the trained random forest model and code for hyperparameter optimization. The approach involves extracting time series data using the calculate_and_save_features function from the Tsfresh_data_extraction folder. The extracted data, along with different hyperparameter combinations, serves as input to the pretrained random forest model. The model predicts MSE, and the combination with the lowest MSE is considered optimal. This approach is applied to Air Quality Data.

3. Regression Models
The Regression_Models folder houses Python files for data preprocessing and model testing:

data_preprocessing.py: This file combines datasets from the Generated_datasets_for_Regressor_Model and Generated_time_series_data folders for training and predicting MSE.

Testing_on_percentage_renewable_data.ipynb: Utilizes carbon intensity data for training and renewable energy data for testing.

Testing_with_wholedata.py: Uses all available datasets for training and testing. The trained random_forest_model.pkl is obtained from this code file.

4. Standard Approach
The Standard_Approach folder is dedicated to training LSTM models using various combinations of hyperparameters, including sequence length and scaler type. The results are compared, and the best hyperparameter combination is selected.

5. Tsfresh Data Extraction
This folder defines the time series data extraction function, utilizing the Tsfresh library.

Through these organized folders and files, the project implements and evaluates different approaches for optimizing hyperparameters in renewable energy forecast models, contributing to advancements in sustainability and energy efficiency.
