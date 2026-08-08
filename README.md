# ⚡ Power Consumption Prediction in Zone 3

## 📌 Project Overview

This project focuses on predicting **electricity consumption in Zone 3** using historical power consumption, weather conditions, and time-based features.

The project was completed as part of a Machine Learning project with **First Quadrant Labs**.

The goal was to build and compare regression models and identify the best-performing model for predicting Zone 3 power consumption.

---

## 🎯 Business Problem

Accurate electricity consumption prediction can help organizations improve:

- Energy management
- Resource planning
- Electricity distribution
- Demand forecasting
- Operational efficiency

Power consumption can be influenced by factors such as weather conditions, time of day, day of the week, and historical electricity usage.

This project uses these factors to develop a predictive Machine Learning model.

---

## 📊 Dataset Overview

The dataset contains:

- **12,321 records**
- **9 original features**
- **13 features used for modeling after feature engineering**
- **Target Variable:** `PowerConsumption_Zone3`

### Original Features

| Feature | Description |
|---|---|
| `Datetime` | Date and time of the observation |
| `Temperature` | Temperature measurement |
| `Humidity` | Humidity level |
| `WindSpeed` | Wind speed |
| `GeneralDiffuseFlows` | General diffuse solar radiation |
| `DiffuseFlows` | Diffuse solar radiation |
| `PowerConsumption_Zone1` | Power consumption in Zone 1 |
| `PowerConsumption_Zone2` | Power consumption in Zone 2 |
| `PowerConsumption_Zone3` | Power consumption in Zone 3 — Target |

---

## 🧹 Data Cleaning & Preprocessing

The following steps were performed:

- Examined the dataset structure
- Checked data types
- Checked missing values
- Checked duplicate records
- Converted the `Datetime` column into datetime format
- Prepared the data for exploratory analysis and Machine Learning

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

These features helped capture temporal patterns in electricity consumption.

---

## 🔍 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand:

- Power consumption distributions
- Consumption patterns over time
- Relationships between weather variables and power consumption
- Correlations between numerical features
- Relationships between input variables and the target

### Visualization Tools

- Matplotlib
- Seaborn

---

## 🤖 Machine Learning Models

Three regression models were developed and compared:

1. **Linear Regression**
2. **Decision Tree Regressor**
3. **Random Forest Regressor**

### Evaluation Metrics

The models were evaluated using:

- **MAE — Mean Absolute Error**
- **RMSE — Root Mean Squared Error**
- **R² Score**

---

## 🏆 Model Performance

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 1209.87 | 1493.89 | 0.8786 |
| Decision Tree | 366.97 | 586.83 | 0.9813 |
| **Random Forest** | **259.94** | **395.67** | **0.9915** |

### 🥇 Best Model: Random Forest Regressor

The Random Forest model achieved:

- **MAE:** 259.94
- **RMSE:** 395.67
- **R² Score:** 0.9915

The model explained approximately **99.15% of the variance** in the test-set target values.

---

## 🔎 Feature Importance

Feature importance was analyzed using the Random Forest model to understand which variables contributed most to predicting Zone 3 electricity consumption.

This helped provide additional insights into the factors associated with power demand.

---

## 📈 Key Findings

- Time-based features helped capture consumption patterns.
- Tree-based models performed better than Linear Regression.
- Random Forest achieved the best overall predictive performance.
- Historical power consumption variables provided important predictive information.
- Feature importance analysis helped identify the variables most useful for prediction.

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
- Exploratory Data Analysis
- Feature Engineering

---

- ## 📂 Project Files

- 📓 [Jupyter Notebook](./Power_Consumption_Prediction.ipynb)
- 📊 [PowerPoint Presentation](./Power_Consumption_Prediction.pptx)
- 📁 [Dataset](./powerconsumption.csv)
> Note: The presentation filename contains spaces. You can rename it on GitHub to `Power_Consumption_Prediction.pptx` to make the link cleaner.

---

## 📁 Project Structure

```text
Power-Consumption-Prediction/
│
├── README.md
├── Power_Consumption_Prediction.ipynb
├── Power_Consumption_Prediction.pptx
│
└── dataset/
    └── powerconsumption.csv

## 🎓 Skills Demonstrated

Data Cleaning
Exploratory Data Analysis
Data Visualization
Feature Engineering
Regression
Machine Learning
Model Evaluation
Feature Importance
Python Programming
Business-oriented Data Analysis

👩‍💻 Author
Ramjot Kaur
Aspiring Data Analyst with hands-on experience in:
Python | SQL | Excel | Tableau | Power BI | Machine Learning | Data Visualization
Project: Power Consumption Prediction in Zone 3
Organization: First Quadrant Labs
