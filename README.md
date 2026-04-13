# 🏡 House Price Prediction using Machine Learning

An end-to-end machine learning project that predicts housing prices in Bengaluru using multiple regression models, achieving an R² score of 0.82 with Linear Regression.

##  Problem Statement

Accurate house price prediction is crucial for buyers, sellers, and real estate investors. This project aims to build a regression model that estimates property prices based on features like area, location, and number of bedrooms.


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

- Linear Regression performed best with an R² score of 0.82, indicating strong linear relationships in the dataset.
- Random Forest and XGBoost showed competitive performance but slightly lower generalization.
- Decision Tree underperformed due to overfitting.


## Key Steps
- Cleaned messy total_sqft (ranges, wrong units)
- Engineered bhk and price_per_sqft features
- Removed outliers using statistical methods
- One hot encoded 248 locations
- Tuned Random Forest with GridSearchCV

## Methodology

- Cleaned inconsistent `total_sqft` values (ranges and units)
- Removed outliers using statistical thresholds
- Engineered features such as `bhk` and `price_per_sqft`
- Applied One-Hot Encoding for categorical location data (248 categories)
- Trained multiple regression models and optimized Random Forest using GridSearchCV

## How to Run
1. Clone the repo
2. pip install -r requirements.txt
3. Open notebooks/house_price_prediction.ipynb

## Model
The trained model file (.pkl) is not included due to file size.
To generate it, run all cells in the notebook — 
the model will be saved automatically.

## Future Improvements

- Deploy model using Streamlit for real-time predictions
- Use more advanced feature engineering
- Collect more data to improve model generalization

## 📌 Key Learnings

- Handling messy real-world datasets
- Importance of feature engineering
- Model comparison and evaluation techniques
