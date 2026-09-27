# Housing Price Prediction - Final Data Science Project

## Problem Statement
Analyze a housing dataset and build a model to predict house prices 
based on features like area, bedrooms, bathrooms, and amenities.

## Dataset
- **Source:** Kaggle (Housing Price Dataset)
- **Size:** 545 rows, 13 columns

## 1. Data Preparation
- No missing values or duplicate rows found
- Data types were correct; categorical columns converted to `category` type
- Outliers found in Price and Area (retained as genuine data)
- Saved as `cleaned_housing_data.csv`

## 2. Exploratory Data Analysis
Created visualizations: price distribution, area vs price, bedrooms vs 
average price, furnishing status vs price, and a correlation heatmap.

**Key Insights:**
1. Price distribution is right-skewed (most houses 30-60 lakhs)
2. Area and Price have a strong positive relationship
3. More bedrooms generally means higher average price
4. Furnished houses are priced higher than unfurnished ones
5. Area has the strongest correlation with Price

## 3. Modeling and Evaluation
Trained and compared two models to predict Price:

| Model              | MAE       | RMSE       | R² Score |
|---------------------|-----------|------------|----------|
| Linear Regression   | 979,680   | 1,331,071  | 0.649    |
| Random Forest       | 1,025,290 | 1,401,263  | 0.612    |

**Final Model:** Linear Regression (better performance, likely due to 
the dataset's linear pattern and small size).

## Limitations
- Models explain only ~60-65% of price variation
- Dataset lacks key factors like location and property age
- Small dataset size limits complex model performance

## Conclusion
Completed the full data science pipeline — cleaning, analysis, and 
modeling. Linear Regression proved to be a solid baseline model, with 
room for improvement through better features and advanced algorithms.

## Files
- `housing.csv` — Original dataset
- `cleaned_housing_data.csv` — Cleaned dataset
- `Final_Housing_Project.ipynb` — Full project notebook
- `README.md` — This file