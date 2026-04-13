# house-price-prediction
ML project to predict house prices using Scikit-learn and XGBoost

# 🏠 House Price Prediction

## Overview
End-to-end Machine Learning project to predict house 
prices in Bengaluru using regression models.

## Dataset
- Source: Kaggle - Bengaluru House Price Data
- Rows after cleaning: 9,745

## Tech Stack
Python, Pandas, NumPy, Matplotlib, Seaborn, 
Scikit-learn, XGBoost, Pickle

## Models & Results
| Model              | R² Score | MAE   | RMSE  |
|--------------------|----------|-------|-------|
| Linear Regression  | 0.8203   | 17.86 | 33.23 |
| Tuned RandomForest | 0.7554   | 16.57 | 38.77 |
| XGBoost            | 0.7366   | 16.55 | 40.23 |
| Decision Tree      | 0.4399   | 20.33 | 58.66 |

## Key Steps
- Cleaned messy total_sqft (ranges, wrong units)
- Engineered bhk and price_per_sqft features
- Removed outliers using statistical methods
- One hot encoded 248 locations
- Tuned Random Forest with GridSearchCV

## How to Run
1. Clone the repo
2. pip install -r requirements.txt
3. Open notebooks/house_price_prediction.ipynb

## Model
The trained model file (.pkl) is not included due to file size.
To generate it, run all cells in the notebook — 
the model will be saved automatically.
