# Real Estate Price Intelligence

Predicting **house sale prices** and **apartment rent prices** using two independently tuned regression models, deployed as an interactive Streamlit web app.

🔗 **Live demo:** [real-estate-price-intelligence.streamlit.app](https://real-estate-price-intelligence.streamlit.app/)

---

## Problem Statement

Buyers, renters, and agents often lack a quick way to sanity-check whether a listed price is reasonable given a property's features. This project builds two separate regression pipelines — one for house sale prices, one for apartment rent — and wraps them in a simple web interface where a user can input property characteristics and get an instant price estimate.

## Datasets

- **House prices:** Kaggle house price dataset (features include overall quality, square footage, bathrooms, etc.)
- **Apartment rent:** Kaggle apartment rent dataset

*(https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)*
.
*(https://www.kaggle.com/datasets/plutozehatescoding/apartments-for-rent-classified)*

## Approach

1. **Exploratory Data Analysis (EDA)** — examined distributions, correlations, and outliers across both datasets
2. **Feature Engineering** — selected and transformed relevant predictors for each target
3. **Log Transformation** — applied to target variables to reduce skew and stabilize variance
4. **Model Comparison** — evaluated multiple regression algorithms per dataset to identify the best performer
5. **Deployment** — packaged the winning models into a two-tab Streamlit app for interactive predictions

## Results

| Target | Best Model | Metric | Score |
|---|---|---|---|
| House Sale Price | Ridge Regression | RMSE / R² | *add value* |
| Apartment Rent | Random Forest | RMSE / R² | *add value* |

Ridge regression outperformed other models on the house price dataset, likely due to its regularization handling multicollinearity among features well. Random Forest performed best on the rent dataset, capturing non-linear relationships that a linear model missed.

*(Replace the placeholders above with your actual evaluation numbers — this table is the first thing most recruiters check.)*

## Tech Stack

- **Language:** Python
- **ML:** scikit-learn (Ridge Regression, Random Forest)
- **Data Handling:** pandas, numpy
- **Web App:** Streamlit
- **Model Serialization:** joblib

## Project Structure
