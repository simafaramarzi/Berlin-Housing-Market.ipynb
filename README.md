#  Berlin Housing Market Analysis

An end-to-end data analysis and machine learning project that explores the Berlin housing market and develops a predictive model for estimating residential property prices.

---

## 📌 Project Overview

Understanding the factors that influence housing prices is essential for buyers, sellers, investors, and real estate professionals.

This project analyzes residential property listings in Berlin to identify the key drivers of property prices through exploratory data analysis (EDA), feature engineering, and predictive modeling.

The complete workflow includes:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Regression Modeling
- Model Evaluation

---

## 🎯 Business Objective

The objective of this project is to:

- Understand pricing patterns in the Berlin housing market
- Identify the most influential property characteristics
- Build a machine learning model capable of estimating house prices
- Demonstrate a complete data analysis workflow from raw data to business insights

---

## 📂 Dataset

**Dataset:** BerlinHousing4049.csv

The dataset contains residential property listings with features such as:

- Property Price
- Living Area
- Number of Bedrooms
- Construction Year
- Property Characteristics

---

## 🛠 Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- Jupyter Notebook

---

## 🔧 Data Cleaning

The following preprocessing steps were performed:

- Removed duplicate records
- Imputed missing values using the median
- Converted year-related columns into datetime format
- Removed price outliers using the Interquartile Range (IQR) method

---

## ⚙️ Feature Engineering

To improve model performance:

- Created a **Price per Square Foot** feature
- Standardized numerical variables using **StandardScaler**

---

## 📊 Exploratory Data Analysis

The analysis included:

- Price distribution analysis
- Log transformation of the target variable
- Correlation heatmap
- Scatter plots
- Distribution analysis of numerical variables

---

## 🤖 Machine Learning

A Linear Regression model was developed to predict property prices.

### Model Performance

| Metric | Result |
|---------|--------|
| R² Score | **0.47** |

The model explains approximately **47% of the variance** in housing prices using the available property features.

---

## 💡 Key Insights

- Property size is the strongest predictor of price.
- Larger homes generally command higher prices.
- Log transformation reduced skewness and improved data distribution.
- Removing extreme outliers increased model stability.
- Several property characteristics show moderate correlations with price, indicating that additional location-based features could further improve prediction accuracy.

---

## 📸 Project Preview

*(Add screenshots here)*

Example:

![Correlation Heatmap](images/correlation_heatmap.png)

![Price Distribution](images/price_distribution.png)

---

## 🚀 How to Run

Clone the repository

```bash
git clone https://github.com/yourusername/Berlin-Housing-Market.git
```

Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
Berlin Housing Market.ipynb
```

---

## 🔮 Future Improvements

- Compare multiple regression algorithms (Random Forest, XGBoost)
- Perform hyperparameter tuning
- Apply cross-validation
- Incorporate location-based features
- Deploy the model as an interactive web application using Streamlit

---

## 👤 Author

**Sima Faramarzi**

M.Sc. Data Science | Python | SQL | Machine Learning | Data Analytics- Property size is the strongest predictor of price.
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
