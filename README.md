# Air Quality Index (AQI) Analysis and Prediction

## Overview

This project uses Machine Learning to predict the Air Quality Index (AQI)
from air pollutant concentrations. It uses Python and Scikit-learn to
build a Random Forest Regression model, evaluate its performance, and
predict AQI values for new pollutant measurements.

## Objectives

- Analyze an air quality dataset containing 18,265 records and 13 columns.
- Select relevant pollutant concentrations as input features.
- Split the dataset into training and testing sets.
- Train a Random Forest Regression model to predict AQI.
- Evaluate model performance using MAE, MSE, and R² score.
- Visualize actual versus predicted AQI values.
- Analyze pollutant feature importance.
- Predict AQI using newly entered pollutant concentrations.

## Dataset

The dataset contains 18,265 records and 13 columns, including city,
date and time, pollutant concentrations, AQI, and AQI category.

### Input Features

The model uses the following nine pollutant concentrations:

- PM2.5
- PM10
- NO
- NO2
- NOx
- NH3
- CO
- SO2
- O3

### Target Variable

- **AQI:** Air Quality Index

The `City`, `Datetime`, and `AQI_Bucket` columns are present in the
dataset but are not used as input features in the current model.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab / Jupyter Notebook

## Machine Learning Workflow

1. Load the air quality dataset.
2. Inspect the dataset structure and data types.
3. Select pollutant concentrations as input features and AQI as the target.
4. Split the data into training and testing sets using an 80:20 ratio.
5. Train a Random Forest Regressor with 100 decision trees.
6. Predict AQI values for the test dataset.
7. Evaluate predictions using regression metrics.
8. Visualize model predictions and feature importance.
9. Predict AQI for new pollutant measurements.

## Model Performance

The Random Forest Regression model achieved the following results
on the test dataset:

| Evaluation Metric | Result |
|-------------------|-------:|
| Mean Absolute Error (MAE) | 1.0383 |
| Mean Squared Error (MSE) | 40.4105 |
| R² Score | 0.99697 |

### Evaluation Metrics

- **MAE:** Measures the average absolute difference between actual
  and predicted AQI values.
- **MSE:** Measures the average squared prediction error.
- **R² Score:** Measures how well the model explains variation in
  the target values.

The model achieved an R² score of approximately 0.997 on the test set.
These results describe performance on the current data split and
should be validated further before making claims about generalization
to unseen cities or future dates.

## Visualizations

The notebook includes:

- **Actual vs. Predicted AQI:** Compares the model's predictions
  with the actual AQI values.
- **Feature Importance:** Shows the relative importance assigned
  to each pollutant feature by the trained Random Forest model.

## AQI Prediction for New Inputs

The notebook allows users to enter pollutant concentrations for
PM2.5, PM10, NO, NO2, NOx, NH3, CO, SO2, and O3.

The trained Random Forest model then predicts an AQI value based
on these inputs.

## How to Run

1. Open the project notebook in Google Colab or Jupyter Notebook.
2. Upload or load the required air quality dataset.
3. Run the notebook cells in sequence.
4. Review the model evaluation metrics and visualizations.
5. Enter pollutant concentrations in the new AQI prediction section
   to obtain a prediction.

Required Python libraries:

- pandas
- numpy
- matplotlib
- scikit-learn

## Project Status

The initial Random Forest Regression model has been implemented,
evaluated, and tested with new pollutant inputs.

The Jupyter Notebook will be uploaded to this repository.

## Future Improvements

- Compare Random Forest Regression with Linear Regression and
  other regression algorithms.
- Validate the model using additional train-test splits and
  appropriate cross-validation.
- Investigate potential data leakage and correlations among
  pollutant concentrations and AQI.
- Evaluate performance on unseen cities and different time periods.
- Develop an interactive interface for AQI prediction.

## Author

Devasri M

## License

A license has not yet been specified.
