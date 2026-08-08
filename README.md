# ⚡ Power Consumption Prediction in Zone 3

## 📌 Project Overview

This project focuses on predicting electricity consumption in **Zone 3** using historical power consumption data, weather conditions, and time-based features.

The project was completed as a Machine Learning research project with **First Quadrant Labs**.

The objective is to develop a regression model capable of accurately predicting `PowerConsumption_Zone3` and identifying the factors that influence electricity demand.

---

## 🎯 Business Problem

Accurate power consumption forecasting can help improve energy management, resource allocation, and electricity distribution.

Power demand can vary based on:

- Weather conditions
- Time of day
- Day of the week
- Seasonal patterns
- Historical electricity consumption

This project uses these factors to build a predictive model for Zone 3 power consumption.

---

## 📊 Dataset

The dataset contains:

- **12,321 observations**
- **9 original features**
- No missing values

### Target Variable

`PowerConsumption_Zone3`

### Original Features

| Feature | Description |
|---|---|
| Datetime | Date and time of the observation |
| Temperature | Temperature measurement |
| Humidity | Humidity level |
| WindSpeed | Wind speed |
| GeneralDiffuseFlows | General diffuse solar radiation |
| DiffuseFlows | Diffuse solar radiation |
| PowerConsumption_Zone1 | Power consumption in Zone 1 |
| PowerConsumption_Zone2 | Power consumption in Zone 2 |
| PowerConsumption_Zone3 | Power consumption in Zone 3 |

---

## 🧹 Data Cleaning & Preprocessing

The following preprocessing steps were performed:

- Checked dataset structure
- Checked missing values
- Checked duplicate records
- Reviewed data types
- Converted `Datetime` into datetime format
- Prepared the dataset for exploratory analysis and machine learning

The dataset contained **no missing values**.

---

## ⚙️ Feature Engineering

Time-based features were extracted from the `Datetime` column:

- `Year`
- `Month`
- `Day`
- `Hour`
- `DayOfWeek`
- `Weekend`

These features help the models capture temporal patterns in electricity consumption.

---

## 🔍 Exploratory Data Analysis

EDA was performed to understand:

- Distribution of Zone 3 power consumption
- Relationship between temperature and power consumption
- Consumption patterns over time
- Relationships between numerical variables
- Correlations between features and the target variable

Visualizations were created using:

- Matplotlib
- Seaborn

---

## 🤖 Machine Learning Models

Three regression models were developed and evaluated:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor

### Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## 🏆 Model Performance

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 1209.87 | 1493.89 | 0.8786 |
| Decision Tree | 366.97 | 586.83 | 0.9813 |
| Random Forest | **259.94** | **395.67** | **0.9915** |

### 🥇 Best Model

The **Random Forest Regressor** achieved the best performance with:

- **MAE:** 259.94
- **RMSE:** 395.67
- **R² Score:** 0.9915

This indicates that the Random Forest model explained approximately **99.15% of the variance** in the test-set target values.

---

## 🔎 Feature Importance

Feature importance was analyzed using the Random Forest model to understand which variables contributed most to predicting Zone 3 power consumption.

This provides additional insight into the factors associated with electricity demand.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Machine Learning

---

## 📁 Project Structure

```text
Power-Consumption-Prediction/
│
├── Power_Consumption_Prediction.ipynb
├── Power_Consumption_Prediction.pptx
├── README.md
└── dataset/
    └── powerconsumption.csv

## 👩‍💻 Author

### Ramjot Kaur

Aspiring Data Analyst with hands-on experience in Python, SQL, Excel, Tableau, Power BI, Data Visualization, and Machine Learning.

**Project:** Power Consumption Prediction in Zone 3  
**Organization:** First Quadrant Labs
