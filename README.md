# Airbnb Housing Price Prediction
Project Overview

This project aims to predict Airbnb housing prices using machine learning techniques. By analyzing a dataset of over 74,000 Airbnb listings, this project demonstrates the application of Random Forest Regressor and Ridge Regression to real-world pricing data.

The project focuses on understanding the relationships between numeric, categorical, and geographical features in the dataset and uses them to predict the log-transformed and actual prices of Airbnb listings. The dataset is from https://www.kaggle.com/datasets/rupindersinghrana/airbnb-price-dataset/data.

## Dataset

Source: Kaggle – Airbnb Price Dataset

Number of entries: 74,111

Features: 29, including numeric, categorical, text, and geographic data

Key Features Used in Modeling

Numeric: accommodates, bathrooms, bedrooms, beds, review_scores_rating, number_of_reviews

Categorical: property_type, room_type, cancellation_policy, bed_type, city

Target Variable: log_price (logarithmic form of the price)

## Data Preprocessing

Missing values in numeric columns filled with median values

Missing categorical values filled with "Unknown"

One-hot encoding applied to categorical variables

Numeric and categorical features combined into a sparse matrix for efficient modeling

## Machine Learning Models

Two models were implemented:

Random Forest Regressor

Captures non-linear relationships between features

Parameters: 100 decision trees, max depth = 15

Ridge Regression

Linear regression with L2 regularization

Helps prevent overfitting and serves as a linear baseline

## Evaluation Metrics

Models were evaluated using:

R² Score – proportion of variance explained

RMSE (Root Mean Squared Error) – measures average prediction error

MAE (Mean Absolute Error) – average absolute error

Results

Random Forest Regressor:

R²: 0.605

RMSE: 0.45

MAE: 0.34

Ridge Regression:

R²: 0.561

RMSE: 0.48

MAE: 0.36

## Observation: Random Forest outperformed Ridge Regression due to its ability to capture non-linear relationships between features and target.

Feature Analysis

The top 20 important features from the Random Forest model were visualized to understand which features contributed most to Airbnb pricing predictions.
