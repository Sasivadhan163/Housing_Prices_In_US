🏡 Housing Price Prediction Using Machine Learning

This project analyzes a large U.S. housing dataset and builds machine learning models to predict home prices using property features, geographic information, and socioeconomic factors.

It includes data cleaning, exploratory data analysis (EDA), feature engineering, model training, model comparison, and interpretable insights.

<br>
📁 Dataset Overview

The dataset contains 39,000+ homes across the U.S., with features including:

Beds

Baths

Living Space (sq ft)

Median Household Income

Zip Code Population

Zip Code Density

Latitude / Longitude

City

County

State

Target variable: Price

<br>
🧹 Data Cleaning

Removed 962 duplicate rows

Fixed missing values (median imputation)

Verified correct data types

Examined and handled outliers

Cleaned text/categorical columns

Ensured dataset readiness for modeling

<br>
📊 Exploratory Data Analysis (EDA)

Visualizations included:

Price distribution (raw + log)

Scatter plots:

Living Space vs Price

Median Income vs Price

Baths / Beds vs Price

Correlation heatmap

Geographic feature distributions

<br>
Key EDA Findings

Home prices are heavily right-skewed → log transform improves clarity

Strongest correlations:
✔ Living Space
✔ Baths
✔ Median Household Income

Weakest correlations:
✖ Zip Code Population
✖ Zip Code Density

Location (City, County, State) has tremendous influence on price

<br>
🛠 Feature Engineering

One-hot encoded categorical features (City, County, State → ~300+ new columns)

Dropped non-predictive columns (Address, Zip Code)

Scaled numeric features with StandardScaler

Final dataset contained ~370 engineered features

<br>
🤖 Machine Learning Models

Two supervised regression models were built and compared:

1️⃣ Random Forest Regressor

Strong baseline model

Handles nonlinear patterns well

Provides feature importance

Good performance but limited on high variance data

2️⃣ XGBoost Regressor (Best Model)

Gradient boosting algorithm

Builds trees sequentially, correcting errors

More powerful than Random Forest

Handles complex interactions + outliers

Improved MAE, RMSE, and MAPE

Better generalization

<br>
📈 Model Performance
Metric	Random Forest	XGBoost
MAE	~173k	Lower
RMSE	~629k	Lower
MAPE	~35%	Lower
Notes	Baseline	Best model overall

XGBoost outperformed RandomForest in all metrics.

<br>
🔍 Feature Importance Findings

Top predictors of home price:

Living Space

Median Household Income

Baths

Latitude / Longitude

Top City & County Encodings

This aligns with real estate fundamentals:
⭐ Size + Location are the core determinants of price.

<br>
📉 Actual vs Predicted Analysis

Lower-priced homes predicted accurately (tight clustering)

Spread widens for extremely expensive properties (normal for housing markets)

XGBoost consistently narrows error margins

<br>
🧠 Conclusion

This project demonstrates how machine learning can be applied to real-estate price prediction through:

robust data cleaning

smart feature engineering

strong modeling techniques

effective model comparison

interpretable results

Final Selected Model:
🔥 XGBoost Regressor — highest accuracy and best generalization.

<br>
🚀 Future Enhancements

Hyperparameter tuning for XGBoost

SHAP for model explainability

Price range segmentation (low / mid / luxury)

Geospatial analysis (distance to city center, highways, etc.)

Interactive dashboard (Streamlit)

<br>
📎 Technologies Used

Python

Pandas & NumPy

Scikit-Learn

XGBoost

Matplotlib & Seaborn

Jupyter Notebook

### 👨‍💻 **Author**
**Sasivadhan Kandregula**  
Master’s in Computer Science | Seattle University  
GitHub: [Sasivadhan163](https://github.com/Sasivadhan163)

**Koushika Chappidi**  
Master’s in Computer Science | Pace University  
GitHub: [koushikachappidi-3](https://github.com/koushikachappidi-3)

