# House Price Prediction using Machine Learning

## Overview

This project predicts house prices based on various property features such as area, bedrooms, bathrooms, stories, parking availability, furnishing status, and other amenities. The objective is to build regression models that estimate property prices and identify the factors that have the greatest impact on housing costs.

## Problem Statement

Real estate buyers and sellers often rely on manual comparisons and market assumptions to estimate property values. This project applies machine learning techniques to predict house prices accurately and analyze the features that influence pricing decisions.

## Dataset

* Dataset: Housing Prices Dataset
* Source: Kaggle
* File Used: `Housing.csv`
* Total Records: 545
* Features Include:

  * Area
  * Bedrooms
  * Bathrooms
  * Stories
  * Parking
  * Main Road Access
  * Guest Room
  * Basement
  * Air Conditioning
  * Hot Water Heating
  * Preferred Area
  * Furnishing Status

## Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

## Project Workflow

### 1. Data Exploration

* Loaded and inspected the dataset
* Checked dataset dimensions
* Identified target and feature variables
* Analyzed data types and missing values

### 2. Data Preprocessing

* Removed duplicate records
* Handled categorical variables using One-Hot Encoding
* Prepared features for machine learning models

### 3. Model Development

Two regression models were implemented:

#### Linear Regression

* Trained using 80% of the dataset
* Tested on 20% of the dataset

#### Random Forest Regressor

* Implemented for performance comparison
* Evaluated using the same train-test split

### 4. Model Evaluation

Evaluation metrics used:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

#### Results

| Model                    | MAE          | RMSE         | R² Score |
| ------------------------ | ------------ | ------------ | -------- |
| Linear Regression        | 1,029,305.71 | 1,413,204.62 | 0.6049   |
| Random Forest Regression | 1,104,206.00 | 1,496,229.00 | 0.5571   |

### Best Performing Model

Linear Regression achieved the highest R² Score of 0.605 and provided the best overall performance for this dataset.

## Visualizations

The project includes:

* House Price Distribution Histogram
* Correlation Heatmap
* Actual vs Predicted Price Scatter Plot
* Feature Importance Analysis

## Key Findings

* Bathrooms had the strongest influence on house prices.
* Air conditioning and hot water heating significantly increased property value.
* Main road access and basement availability positively affected pricing.
* Linear Regression outperformed Random Forest Regression on this dataset.
* Property amenities showed a stronger impact on pricing than expected.

## Repository Structure

```text
HousePricePrediction/
│
├── analysis.ipynb
├── Housing.csv
├── summary.pdf
│
└── charts/
    ├── price_distribution.png
    ├── correlation_heatmap.png
    ├── actual_vs_predicted.png
    └── feature_importance.png
```

## Future Improvements

* Hyperparameter tuning
* Cross-validation
* Advanced ensemble models
* Deployment using Streamlit
* Real-time house price prediction application

## Author

Madhu Varshini

Machine Learning | Data Analytics | Artificial Intelligence
