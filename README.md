# Product Demand Forecasting with Linear Regression

## Project Description

Demand forecasting is a key problem in inventory management and operational planning. Accurate demand estimates help reduce stockouts, minimize logistics costs, and improve customer service levels.

In this project, a baseline linear regression model is developed to predict daily product demand using pricing, promotion, and time-based features. The main goal is to understand the drivers of demand and establish a solid benchmark for more advanced models.

---

## Objectives

- Predict daily product demand.
- Analyze the impact of price, promotions, and seasonality.
- Build an interpretable baseline model.
- Evaluate model performance in a realistic future-prediction scenario.

---

## Dataset

The project uses a synthetic dataset designed to simulate realistic retail demand behavior.

**Variables:**

| Variable | Description |
|--------|-------------|
| `date` | Daily date |
| `price` | Product price |
| `promotion` | Promotion indicator (0 = no, 1 = yes) |
| `demand` | Units sold (target variable) |

---

## Data Science Approach

1. Exploratory Data Analysis (EDA).
2. Temporal feature engineering.
3. Time-based train/test split.
4. Feature scaling without data leakage.
5. Baseline linear regression modeling.
6. Business-oriented evaluation metrics.
7. Model interpretation.

---

## Feature Engineering

- Day of week
- Month
- Lagged demand (1-day lag)

---

## Model

- Model: Linear Regression
- Purpose: Baseline model
- Why: High interpretability and ease of communication with business stakeholders

---

## Evaluation Metrics

- MAE
- RMSE
- R²

---

## Key Insights

- Promotions show the largest marginal impact on demand when they occur.
- Lagged demand captures structural temporal dependence and demand continuity.
- Price has a negative relationship with demand, consistent with economic theory.
- The model captures overall trends but struggles with extreme demand spikes.

---

## Limitations

- Linear regression cannot model non-linear relationships.
- External drivers such as holidays or weather are not included.
- Assumes stable relationships over time.

---

## Next Steps

- Apply regularized models (Ridge, Lasso).
- Test non-linear models (Random Forest, XGBoost).
- Explore time-series models (ARIMA, Prophet).
- Add external business variables.
- Implement rolling or expanding window validation.

---

## Technologies

- Python
- pandas, numpy
- matplotlib
- scikit-learn

---

## Author

**Immani Navor Trejo Rojas**  
Portfolio project focused on Business-Oriented Data Science.

