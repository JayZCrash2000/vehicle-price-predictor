
#  Vehicle Price Predictor

A machine learning project to predict used vehicle prices based on features like brand, model, mileage, fuel type, and year of manufacture. Built with real-world data preprocessing, exploratory data analysis, and multiple ML models with hyperparameter tuning.

---

##  Problem Statement

Used car pricing is highly variable and often opaque. This project builds a regression pipeline that predicts the resale price of a vehicle given its specifications — helping buyers, sellers, and dealerships make data-driven decisions.

---

##  Tech Stack

- **Python** — Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Models** — Linear Regression, Random Forest, Gradient Boosting (XGBoost)
- **Evaluation** — RMSE, MAE, R² Score

---

##  Project Structure

```
vehicle-price-predictor/
│
├── vehicle_price_predictor.ipynb   # Main notebook (EDA + modeling)
├── requirements.txt                 # Dependencies
└── README.md
```

---

##  What's Inside the Notebook

1. **Data Loading & Overview** — shape, dtypes, null values
2. **Exploratory Data Analysis (EDA)**
   - Price distribution
   - Correlation heatmap
   - Feature-wise box plots
3. **Data Preprocessing**
   - Handling missing values
   - Encoding categorical features
   - Feature engineering (car age from year)
   - Train-test split + scaling
4. **Model Training**
   - Linear Regression (baseline)
   - Random Forest Regressor
   - Gradient Boosting / XGBoost
5. **Evaluation & Comparison**
   - RMSE, MAE, R² for all models
   - Feature importance plot
6. **Insights & Conclusions**

---

##  Results

| Model | R² Score | RMSE |
|---|---|---|
| Linear Regression | ~0.72 | ~1.8L |
| Random Forest | ~0.89 | ~1.1L |
| Gradient Boosting | ~0.91 | ~0.95L |

> *Results based on synthetic dataset mimicking real used car market data.*

---

##  How to Run

```bash
pip install -r requirements.txt
jupyter notebook vehicle_price_predictor.ipynb
```

---

##  Key Findings

- Car **age** and **mileage** are the strongest predictors of price depreciation
- **Diesel cars** retain value longer than petrol in the Indian market
- **Brand premium** (luxury vs economy) adds significant non-linear variance
- Gradient Boosting outperforms Linear Regression by ~26% in R²

---

##  Author

**Jeet Kumar** — [GitHub](https://github.com/JayZCrash2000)
