# Berlin Housing Market Analysis

A regression analysis of Berlin real estate listings to identify which factors most influence property prices, and to build a predictive pricing model.

## Result

Linear regression model: **R² = 0.47** — explaining about 47% of the variance in property prices based on the available features.

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

## How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
jupyter notebook "Berlin Housing Market.ipynb"
```

Dataset: `BerlinHousing4049.csv` (included in the repo)

## Tools

Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Statsmodels
