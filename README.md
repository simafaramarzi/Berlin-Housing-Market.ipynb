# Berlin Housing Market Analysis

A regression analysis of Berlin real estate listings to identify which factors most influence property prices, and to build a predictive pricing model.

## Project Overview

This project analyzes Berlin housing listings to understand the factors influencing property prices and develops a machine learning model capable of estimating property values based on property characteristics.

The project covers the complete data analysis workflow, including data cleaning, exploratory data analysis (EDA), feature engineering, predictive modeling, and visualization.

## Business Objective

The objective is to help real estate professionals and potential buyers better understand pricing patterns within the Berlin housing market and identify the most influential property characteristics affecting price.

## Result

The Linear Regression model achieved:

- R² Score: 0.47
- The model explains approximately 47% of the variance in housing prices.
- Results indicate that property size, number of bedrooms, and location-related variables contribute significantly to price prediction.


## What I Did

1. **Data Cleaning**
   - Imputed missing values using the median to preserve distribution integrity
   - Removed duplicate entries
   - Converted year fields to datetime for time-based analysis
   - Removed statistical outliers in the price column using the IQR method

2. **Feature Engineering**
   - Created `price_per_sqft` as a standardized value metric for comparing properties
   - Scaled numerical features with `StandardScaler` to prepare for modeling

3. **Exploratory Analysis**
   - Log-transformed price distribution to correct for skew
   - Scatter plots of price vs. bedrooms, square footage, and other features
   - Correlation heatmap across all numerical variables

4. **Modeling**
   - Built a linear regression model to predict property price
   - Evaluated performance with R² and residual analysis

## Key Insights

- Larger properties generally command higher prices.
- Property size is the strongest predictor of price.
- Log transformation improved the distribution of the target variable.
- Removing outliers improved model stability.

## Future Improvements

- Compare multiple regression algorithms
- Hyperparameter tuning
- Cross-validation
- Feature selection
- Deploy the model using Streamlit
  
## How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
jupyter notebook "Berlin Housing Market.ipynb"
```

Dataset: `BerlinHousing4049.csv` (included in the repo)

## Tools

Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Statsmodels
