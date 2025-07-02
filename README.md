
# 🗽 NYC Taxi Ride Duration Prediction

This project is focused on predicting the duration of taxi rides in New York City using machine learning. It was developed as part of a data science learning track, using real-world data from the [Kaggle NYC Taxi Trip Duration dataset](https://www.kaggle.com/competitions/nyc-taxi-trip-duration/data).

## 📌 Objective

Build a regression model to predict the ride duration (in seconds) based on pickup and dropoff locations, times, and other engineered features.

---

## 📂 Project Structure
* Project-5._NY_taxi_ride_duration.ipynb
* .getignore
* README.md
* submission_gb.csv


The entire analysis and modeling process is contained in the notebook, which is divided into **key sections**:

- **Data Loading and Exploration**  
- **Feature Engineering**  
- **Data Cleaning and Preprocessing**  
- **Model Training and Evaluation**  
- **Feature Importance**  
- **Final Results and Submission Preparation**

---

## 📊 Dataset Overview

The dataset includes over 1 million taxi trips with the following key features:

- `pickup_datetime`, `dropoff_datetime`
- `pickup_longitude`, `pickup_latitude`
- `dropoff_longitude`, `dropoff_latitude`
- `passenger_count`
- `store_and_fwd_flag`
- `trip_duration` (target)

---

## 🧪 Methodology

### 🔧 Feature Engineering
- **Distance calculation** using the haversine formula
- **Datetime features** (hour, weekday, month, etc.)
- **Direction and speed estimates**

### 🚀 Modeling
- Baseline: Linear Regression  
- Advanced models:
  - **Decision Tree**
  - **Random Forest Regressor**
  - **Polynomial Regression**
  - **Gradient Boosting (XGBoost)**

### 🏆 Evaluation
- Metric: **Root Mean Squared Log Error (RMSLE)**
- Cross-validation used to avoid overfitting

---

## 🧠 Key Insights

- **Datetime** and **geospatial features** strongly influence ride duration.
- **XGBoost** outperformed other models with optimized hyperparameters.
- Feature importance analysis revealed trip distance and pickup hour as critical predictors.

---

## ✅ Final Model Performance

| Model           | RMSLE (CV)  |
|----------------|-------------|
| Linear Regression | ~0.59      |
| Random Forest     | ~0.44      |
| XGBoost (tuned)   | **~0.39**  |

---

## 📎 Requirements

- Python 3.8+
- Jupyter Notebook
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- xgboost


