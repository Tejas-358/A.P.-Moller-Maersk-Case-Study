﻿# A.P.-Moller-Maersk-Case-Study
# Sourcing Cost Prediction

This repository contains code for predicting sourcing costs using various machine learning models and time series forecasting techniques. The dataset consists of information about different product types, manufacturers, area codes, sourcing channels, product sizes, and product types.

## Overview

The goal of this project is to develop a model that accurately predicts the sourcing cost for different products based on their attributes. We explore various machine learning models and time series forecasting techniques to achieve this goal.

## Dataset

The dataset contains the following columns:

- ProductType: Type of the product.
- Manufacturer: Manufacturer of the product.
- Area Code: Area code for sourcing.
- Sourcing Channel: Channel through which the product is sourced.
- Product Size: Size of the product.
- Product Type: Type of the product.
- Month of Sourcing: Date of sourcing.
- Sourcing Cost: Cost of sourcing.

## Approaches Explored

### Machine Learning Models:
1. Random Forest Regressor
2. Gradient Boosting Regressor
3. LightGBM
4. Neural Network

### Time Series Forecasting:
1. ARIMA (AutoRegressive Integrated Moving Average)

## Results

### Machine Learning Models:
- Random Forest Regressor:
  - MSE: 1074.02
  - RMSE: 32.77
  
- Gradient Boosting Regressor:
  - MSE: 1427.22
  - RMSE: 37.78
  
- LightGBM:
  - MSE: 1037.75
  - RMSE: 32.21

- Neural Network:
  - MSE: 1168.94
  - RMSE: 34.19

### Time Series Forecasting:
- ARIMA:
  - MSE: 2406.78
  - RMSE: 49.06

Among the machine learning models, LightGBM performs the best in terms of MSE and RMSE, providing a good balance between accuracy and efficiency. ARIMA performs worse compared to the machine learning models.

## Conclusion

Based on the evaluation results, we select LightGBM as the final model for sourcing cost prediction due to its accuracy and efficiency. This model can be deployed in production to predict sourcing costs for new products effectively.
