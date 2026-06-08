# 🌫️ Air Quality Index (AQI) Forecasting using Machine Learning

## 📖 Project Overview

This project implements an end-to-end Machine Learning pipeline for forecasting the Air Quality Index (AQI) using environmental and meteorological data. The system predicts AQI levels by analyzing pollutant concentrations and weather conditions, helping in environmental monitoring and public health awareness.

The project uses multiple regression algorithms including Random Forest, XGBoost, and Gradient Boosting to compare prediction performance and identify the most accurate forecasting model.

---

## 🎯 Objectives

- Predict future AQI values using machine learning.
- Analyze relationships between pollutants and air quality.
- Compare the performance of multiple regression models.
- Visualize AQI trends and feature importance.
- Generate accurate forecasts for environmental monitoring.

---

## 📊 Dataset Features

The dataset contains air quality and weather-related parameters:

- PM2.5
- PM10
- NO₂
- CO
- SO₂
- O₃
- Temperature
- Humidity
- Wind Speed
- Wind Direction
- Atmospheric Pressure
- Time-based Features

Additional engineered features:

- AQI Lag Features
- Rolling Mean Features
- Weekend Indicator

---

## ⚙️ Machine Learning Pipeline

### 1. Data Generation & Collection
- Synthetic AQI dataset based on UCI Air Quality structure.
- Time-series environmental observations.

### 2. Data Preprocessing
- Missing value handling using median imputation.
- Feature scaling and transformation.
- Data cleaning and preparation.

### 3. Feature Engineering
- Lag Features (AQI_lag1, AQI_lag3, AQI_lag6, AQI_lag24)
- Rolling Mean Features
- Temporal Features

### 4. Exploratory Data Analysis (EDA)
- AQI Distribution
- Correlation Heatmaps
- AQI Trends by Hour and Month
- Pollutant Analysis
- AQI Category Distribution

### 5. Model Training
The following models are trained and evaluated:

- Random Forest Regressor
- XGBoost Regressor
- Gradient Boosting Regressor

### 6. Model Evaluation
Performance is measured using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score
- Mean Absolute Percentage Error (MAPE)

### 7. Prediction & Inference
- Predict AQI for new environmental conditions.
- Save trained models for future deployment.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- XGBoost
- Joblib

---

## 📂 Project Structure

```
AQI-Forecasting/
│
├── outputs/
│   ├── aqi_dataset.csv
│   ├── eda_plots.png
│   ├── model_evaluation.png
│   └── summary_report.txt
│
├── models/
│   ├── random_forest.pkl
│   ├── xgboost.pkl
│   └── preprocessor.pkl
│
└── aqi_forecast.py
```

---

## 🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/yourusername/AQI-Forecasting.git
```

2. Install required packages

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost joblib
```

3. Run the project

```bash
python aqi_forecast.py
```

---

## 📈 Results

The models successfully forecast AQI values using pollutant and weather data. Performance comparison helps identify the best-performing model based on RMSE, MAE, MAPE, and R² metrics.

---

## 🌍 Applications

- Air Quality Monitoring
- Smart City Systems
- Environmental Research
- Public Health Advisory Systems
- Pollution Forecasting

---

## 👨‍💻 Author

Machine Learning Project developed for AQI Forecasting and Environmental Data Analysis.
