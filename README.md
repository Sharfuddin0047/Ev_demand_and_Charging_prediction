# EV Adoption Forecasting 🚗🔋

Forecasting the adoption of electric vehicles (EVs) is critical for future-proofing transportation infrastructure. This project builds a predictive model to estimate EV adoption trends using historical data from the Washington State Department of Licensing.

## 📌 Problem Statement

As EV usage grows, there's increasing pressure on public infrastructure—especially charging stations. To address this, we forecast future EV adoption rates based on historical trends.

## 🎯 Goal

Build a **regression-based machine learning model** that predicts the number of electric vehicles using:
- Time series vehicle registration data
- County-level trends
- Vehicle type breakdowns (BEVs, PHEVs)

## 📂 Dataset

**Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/sahirmaharajj/electric-vehicle-population-size-2024/data)

**Features Include:**
- `Date`: Monthly registration date
- `County`, `State`
- `Vehicle Primary Use`: Passenger or Truck
- `BEVs` and `PHEVs` count
- `EV Total`, `Non-EV Total`, `Total Vehicles`
- `Percent Electric Vehicles`

🗓️ Time range: January 2017 to February 2024  
🧾 Size: ~20,000 rows, 10 columns

---

## 🛠️ Technologies Used

- **Language:** Python 3
- **Libraries:** pandas, numpy, matplotlib, seaborn  
- **ML Tools:** scikit-learn, Random Forest Regressor  
- **Model Optimization:** RandomizedSearchCV

---

## 🔍 Data Processing Summary

- Handled missing values in `County` and `State`
- Converted `Date` to datetime format
- Cleaned and converted numeric fields with non-numeric characters
- Detected and capped outliers using IQR in `Percent Electric Vehicles`
- Exploratory analysis on EV distribution by region and use-case

---

## 📈 Model Development

- **Target Variable:** `Electric Vehicle (EV) Total`
- **Features Used:** Date, County, State, BEVs, PHEVs, Total Vehicles
- **Algorithm:** Random Forest Regressor
- **Evaluation Metrics:**
  - R² Score
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)

---

## 📊 Key Insights

- Top EV-adopting counties: Clallam, Jefferson, San Juan
- Truck-based EV adoption lags behind passenger EVs
- EV penetration still low (~2.1% average) but growing steadily

---

## 📎 Outputs

- Data cleaning and visualization plots
- Final trained Random Forest model
- Forecasts for future EV adoption trends

---

## 🚀 Future Improvements

- Integrate charging station availability as a feature
- Explore LSTM or Prophet for time-series forecasting
- Use interactive dashboards (e.g., Plotly, Dash)

---

## 📬 Contact

For queries, feel free to reach out to the project maintainer.  
_Contributors welcome!_

---
