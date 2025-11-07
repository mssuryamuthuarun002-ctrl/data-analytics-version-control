# 🥔 Potato Price Forecasting and Analysis

## 📌 Project Overview
This project focuses on analyzing potato price data along with weather and occasion data to uncover patterns and forecast future price trends. The goal is to help farmers and traders make better decisions using Data Analytics and Time Series Forecasting.  
We developed:
- A **Hybrid ARIMA + XGBoost Model**
- A **Prophet Model with Extra Regressors (Weather & Festival Data)**

These models enable proactive planning and generate **actionable alerts** based on price predictions.

---

## 📂 Dataset Description
| Dataset | Description |
|--------|-------------|
| `Potato price.csv` | Historical modal prices across markets |
| `export.csv` | Weather data (Temperature, Rainfall, Wind, Pressure) |
| `occasions(Sheet1).csv` | List of Indian festivals/occasions with impact ratings |

After preprocessing, time-series data was aligned on the **Date** column.

### **Key Columns**
- Price (Modal Price)
- Date
- Temperature (tavg, tmin, tmax)
- Precipitation (prcp)
- Wind Speed (wspd)
- Pressure (pres)
- Occasion / Festival and its expected market impact

---

## 🛠️ Tools & Technologies Used
| Technology | Purpose |
|-----------|----------|
| Python | Core programming |
| Pandas, NumPy | Data manipulation & cleaning |
| Matplotlib, Seaborn | Visualization |
| statsmodels | ARIMA time-series modeling |
| XGBoost | Non-linear regression modeling |
| Prophet | Forecasting with external regressors |
| Scikit-learn | Model evaluation (RMSE, MAE, R²) |
| Streamlit | Dashboard (initial prototype) |

---

## 🔍 Workflow & Steps
1. Loaded and explored the datasets.
2. Cleaned missing values, handled data inconsistencies, and standardized date format.
3. Expanded festival dataset to map dates and seasonal impact.
4. Merged weather and festival features into the price time series.
5. Built and tuned **ARIMA model** for baseline forecasting.
6. Modeled residual patterns using **XGBoost** (Hybrid Forecasting).
7. Built **Prophet model** using weather + festival indicators.
8. Identified **best selling windows** for farmers.
9. Attempted deployment through a Streamlit dashboard.

---



- Price fluctuations correlate with **season changes and rainfall**.
- Certain **festivals drive temporary demand spikes**, affecting price trends.
- Hybrid ARIMA + XGBoost improved predictive accuracy over ARIMA alone.

---

## ✅ Key Conclusions
- **Weather variables** (especially precipitation and temperature) have a measurable impact on potato price fluctuations.
- **Festival/occasion demand cycles** act as short-term price influencers.
- Forecasting helps **farmers optimize selling time**, reduce uncertainty, and improve income stability.

---

## 🙌 Author
**Surya**  
Data Analytics Enthusiast  
📧 (Optional: Add your email or LinkedIn later)

