
# 🔮 EV Adoption Forecasting – Washington State Counties

This project forecasts the growth of Electric Vehicle (EV) adoption across counties in Washington State. Using time-series machine learning models and historical vehicle registration data, it enables users to interactively explore projected EV trends over the next 3 years.

### 📌 Project Overview

- Uses monthly electric vehicle registration data by county from the Washington State Department of Licensing.
- Builds a regression model to predict future EV counts using lag, trend, and time-based features.
- Deploys an interactive Streamlit dashboard to visualize both monthly and cumulative EV growth.
- Users can explore forecasts by county and compare multiple counties side-by-side.

---

## 🎯 Learning Objectives

- Understand time-series forecasting in the context of regional EV adoption.
- Engineer lag-based and rolling window features for temporal models.
- Tune machine learning models using cross-validation and optimization tools.
- Deploy an interactive dashboard for end-user analysis and insights.

---

## 🧰 Tools & Technologies Used

| Tool/Library        | Version     | Purpose                                               |
|---------------------|-------------|--------------------------------------------------------|
| Python              | 3.11.9      | Core development language                             |
| NumPy               | 1.26.4      | Numerical computing and array operations              |
| Pandas              | 1.5.3       | Data manipulation and time-series transformation      |
| Scikit-learn        | 1.6.1       | Model training, tuning, and evaluation                |
| Matplotlib          | latest      | Data visualization and plotting                       |
| Streamlit           | 1.44.1      | Web-based dashboard and user interface                |
| Joblib              | latest      | Saving and loading trained ML models                  |
| Optuna              | latest      | Hyperparameter optimization                           |
| Jupyter Notebook    | -           | Experimentation and development environment           |

---

## 📈 Methodology

1. **Data Collection & Cleaning**  
   Preprocessed county-level monthly EV registration data.

2. **Feature Engineering**  
   Added lag features, rolling averages, percent changes, and growth slopes.

3. **Model Selection & Training**  
   Random Forest Regressor selected for robustness with non-linear patterns.

4. **Hyperparameter Tuning**  
   Optimized using Optuna for R² performance.

5. **Evaluation**  
   TimeSeriesSplit cross-validation with R², MAE, and RMSE metrics.

6. **Forecasting**  
   Forecasts generated monthly for 3 years using latest historical trends.

7. **Visualization**  
   Streamlit dashboard plots both monthly and cumulative EV forecasts.

---

## 📊 Results

- **MAE:** 0.01  
- **RMSE:** 0.06  
- **R² Score:** 1.00  
- **Top Features:** Lag1 and Lag2 (combined ~65% importance)

> The model demonstrates excellent accuracy, consistency, and generalizability.

---

## 🚀 Streamlit Features

- Select any county to visualize 3-year EV trends.
- Toggle between **monthly** and **cumulative** forecast views.
- Compare EV growth for up to 3 counties simultaneously.
- Styled, responsive dashboard with light/dark adaptive color themes.

---

## 🧠 Future Scope

- Upgrade to deep learning models (e.g., LSTM, GRU, TFT).
- Integrate policy, pricing, and infrastructure data for richer context.
- Enable live updates by connecting to real-time EV datasets.

---

## 📸 Dashboard Preview

![Dashboard Preview](./image.png)

---

## 🔗 Project Repository

GitHub: [EV_Adoption_forecasting_proj](https://github.com/Animofly/EV_Adoption_forecasting_proj)
