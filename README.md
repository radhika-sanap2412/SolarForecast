# SolarForecast
Utilized PVLive API and NASA Power to fetch solar generation and weather variables, performing predictive analysis with machine learning and deep learning models to forecast solar power output.
---

## **Project Overview**

This project aims to predict solar power generation by leveraging:
- Historical solar generation data from the **PVLive API**.
- Weather-related variables (e.g., temperature, wind speed, and solar irradiance) from the **NASA Power API**.

The workflow includes:
1. Data extraction and integration from APIs.
2. Feature engineering (including datetime cyclic encoding).
3. Predictive analysis using multiple models:
   - **Linear Regression**
   - **Random Forest**
   - **XGBoost**
   - **LSTM**

---

## **Key Features**
- **API Integration**:
  - Solar generation data from **PVLive**.
  - Weather variables from **NASA Power**.
- **Feature Engineering**:
  - Cyclic encoding for datetime features.
  - Scaled inputs for models requiring normalization.
- **Modeling**:
  - Comparative analysis of traditional machine learning models and deep learning approaches.
  - Hyperparameter tuning for optimal performance.
- **Evaluation**:
  - Root Mean Squared Error (RMSE).
  - R-squared (\(R^2\)) scores.

---
## **Model Results**
| **Model**         | **Train RMSE** | **Test RMSE** | **Train \(R^2\)** | **Test \(R^2\)** |
|--------------------|----------------|---------------|-------------------|------------------|
| Linear Regression  | 3.0655         | 4.3884        | 0.9664           | 0.8998           |
| Random Forest      | 1.8934         | 4.3184        | 0.9822           | 0.8159           |
| XGBoost            | 0.2781         | 4.1812        | 0.9993           | 0.8274           |
| LSTM               | 4.9861         | 6.5988        | N/A              | N/A              |


---

## **Technologies Used**
- **Python**: Core programming language.
- **Libraries**:
  - Data Processing: `pandas`, `numpy`.
  - Visualization: `matplotlib`, `seaborn`.
  - Machine Learning: `scikit-learn`, `xgboost`.
  - Deep Learning: `TensorFlow` (LSTM model).
- **APIs**:
  - **PVLive** for solar generation data.
  - **NASA Power** for weather variables.

---

## **How to Run**

1. Download the notebook and use it in jupyter/colab
