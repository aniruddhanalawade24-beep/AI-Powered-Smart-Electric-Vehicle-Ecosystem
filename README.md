# 🔋 Smart EV Assistant – README

## 🚀 Project Overview
This project uses machine learning to build a Smart EV Assistant that predicts five key outputs related to electric vehicle charging, battery health, and grid load forecasting. It integrates three datasets to deliver accurate, real-time insights for users and grid operators.

---

## 📦 Datasets Used

1. **EV Charging Pattern Dataset**
   - Charging rate, duration, cost, battery %, temperature, user type, etc.

2. **Battery Health Dataset**
   - Charge/discharge cycles, voltage, temperature, SOH (State of Health), RUL (Remaining Useful Life)

3. **Grid Load Dataset**
   - Power consumption, solar/wind input, grid supply, faults, environmental factors

---

## 🎯 Outputs Predicted

### 1. ⏱️ Charging Time
- **Goal**: Estimate how long the EV will take to charge
- **Model**: Linear Regression
- **Key Features**: Energy Consumed, Charging Rate, Battery Capacity, Charger Type

### 2. 💰 Charging Cost
- **Goal**: Predict cost based on energy usage and time
- **Model**: Random Forest
- **Key Features**: Energy Consumed, Charging Rate, Time of Day, Electricity Price, Charger Type

### 3. 🔋 Battery Health Score (SOH)
- **Goal**: Estimate current battery condition
- **Model**: Random Forest Regression
- **Key Features**: Voltage, Temperature, Cycle Count, Charge/Discharge Stats

### 4. ⏳ Remaining Useful Life (RUL)
- **Goal**: Predict how many cycles or months the battery has left
- **Model**: Time-Series Forecasting (LSTM or Random Forest)
- **Key Features**: SOH, Cycle Count, Temperature, Charging Rate

### 5. ⚡ Grid Load Forecast
- **Goal**: Predict future electricity demand
- **Model**: Time-Series Forecasting (Prophet or LSTM)
- **Key Features**: Power Consumption, Solar/Wind Power, Temperature, Humidity, Fault Indicators

---

## 🧠 Feature Engineering

Custom features created to improve model accuracy:
- `Charging Efficiency = Energy Consumed / Charging Duration`
- `Battery Stress Index = Charging Rate × Temperature`
- `Renewable Ratio = (Solar + Wind) / Grid Supply`

---

## 🛠️ Tools & Libraries
- Python (pandas, scikit-learn, matplotlib, seaborn)
- ML Models: Linear Regression, Random Forest, LSTM, Prophet
- Optional: Streamlit for dashboard interface

---

## 📈 Evaluation Metrics
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

---

---

## 👨‍🔬 Author
Built by **Aniruddha Milind Nalawade**

---
