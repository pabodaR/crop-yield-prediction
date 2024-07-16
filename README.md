# Crop Yield Prediction Model

## Table of Contents
1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
3. [Dataset](#dataset)
4. [Data Preprocessing](#data-preprocessing)
5. [Modeling](#modeling)
6. [Evaluation](#evaluation)
7. [Results](#results)

## Introduction
One of the key metrics in agricultural productivity is crop yield, typically measured in hectograms per hectare (hg/ha). Crop yield is influenced by various factors, including climatic conditions, agricultural practices, and environmental variables. This project aims to predict crop yield using machine learning techniques.

## Project Overview
- **Objective:** Predict crop yield
- **Features:** Data exploration, preprocessing, model selection, evaluation, visualization

## Dataset
- **Source:** https://www.kaggle.com/datasets/patelris/crop-yield-prediction-dataset
- **Description:** The dataset comprises agricultural data with attributes such as Area, Crop name, Year, hg/ha_yield, average rain fall in mm per year, pesticides in tonnes, average temperature.
  
## Data Preprocessing
- Handling missing values
- Handling duplicate values
- Encoding categorical variables]
- Feature engineering

## Modeling
- Models used: Random Forest, XGBoost
- The root mean squared errror (RMSE) value and R^2 value of models were compared to select the most suitable model.

## Evaluation
### Metric: R^2 

| Model                   | Train Accuracy | Test Accuracy |
|-------------------------|----------------|---------------|
| XGBoost                 | 0.9991         | 0.9858        |
| Random Forest           | 0.9981         | 0.9862        |

### Metric: RMSE  

| Model                   | Train Accuracy | Test Accuracy |
|-------------------------|----------------|---------------|
| XGBoost                 | 2596.062       | 10160.974     |
| Random Forest           | 3742.320       | 9996.7925     |

## Results
-   Both XGBoost and Random Forest models perform well in both train and test sets showing good generalization with no overfitting.

-   Random forest model shows lower RMSE on test data than XGBoost.
  
-   Random forest model is recommended for this crop yield prediction task. It provides a good mix of training and testing accuracy without significant overfitting, making it a robust and reliable model for the task.


