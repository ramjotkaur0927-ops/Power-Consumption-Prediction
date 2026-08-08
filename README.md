# ⚡ Power Consumption Prediction in Zone 3

## 📌 Project Overview

This project focuses on predicting **electricity consumption in Zone 3** using historical power consumption, weather conditions, and time-based features.

The project was completed as part of a Machine Learning project with **First Quadrant Labs**.

The main objective was to perform an end-to-end Machine Learning workflow, from data understanding and exploratory data analysis to feature engineering, model building, evaluation, and selection of the best-performing regression model.

---

## 🎯 Objective

The objective of this project is to predict:

**`PowerConsumption_Zone3`**

using historical electricity consumption, weather-related variables, and time-based features.

Accurate power consumption prediction can support:

- Energy management
- Demand forecasting
- Resource planning
- Electricity distribution
- Operational decision-making

---

## 📊 Dataset Overview

The dataset contains:

| Information | Details |
|---|---|
| Records | **12,321** |
| Original Features | **9** |
| Modeling Features | **13** |
| Target Variable | `PowerConsumption_Zone3` |
| Missing Values | **No missing values** |

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

- Dataset structure and data types were examined
- Missing values were checked
- Duplicate records were checked
- `Datetime` was converted into datetime format
- Data was prepared for exploratory analysis
- Features were prepared for Machine Learning

The dataset contained **no missing values**.

---

## ⚙️ Feature Engineering

The `Datetime` feature was used to create additional time-based features:

- `Year`
- `Month`
- `Day`
- `Hour`
- `DayOfWeek`
- `Weekend`

These features help the models capture temporal patterns in electricity consumption.

---

## 🔍 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand:

- Distribution of power consumption
- Power consumption patterns over time
- Relationships between weather variables and electricity consumption
- Correlations between numerical variables
- Relationships between input variables and the target variable

### Visualization Libraries

- Matplotlib
- Seaborn

---

## 🤖 Machine Learning

Three regression algorithms were developed and compared:

### 1. Linear Regression

Used as a baseline regression model.

### 2. Decision Tree Regressor

Used to capture non-linear relationships between features and power consumption.

### 3. Random Forest Regressor

An ensemble learning model used to improve prediction accuracy and capture complex relationships within the data.

---

## 📏 Model Evaluation

The models were evaluated using three metrics:

### MAE — Mean Absolute Error

Measures the average absolute difference between actual and predicted values.

### RMSE — Root Mean Squared Error

Measures prediction error while giving greater weight to larger errors.

### R² Score

Measures how much of the variation in the target variable is explained by the model.

---

## 🏆 Model Performance

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 1209.87 | 1493.89 | 0.8786 |
| Decision Tree Regressor | 366.97 | 586.83 | 0.9813 |
| **Random Forest Regressor** | **259.94** | **395.67** | **0.9915** |

### 🥇 Best Model

**Random Forest Regressor**

Performance:

- **MAE:** 259.94
- **RMSE:** 395.67
- **R² Score:** 0.9915

The Random Forest model achieved the best performance among the evaluated models.

---

## 🔎 Feature Importance

Feature importance was analyzed using the Random Forest model to identify the variables that contributed most to predicting Zone 3 electricity consumption.

This provides useful insight into the factors associated with electricity demand.

---

## 📈 Key Findings

- Time-based features helped capture temporal consumption patterns.
- Tree-based models performed better than Linear Regression.
- Random Forest achieved the highest predictive performance.
- Historical power consumption variables provided important predictive information.
- Feature importance analysis helped identify important predictors of Zone 3 consumption.

---

## 🛠️ Technologies & Tools

**Programming & Analysis**
- Python
- Pandas
- NumPy

**Visualization**
- Matplotlib
- Seaborn

**Machine Learning**
- Scikit-learn
- Regression
- Model Evaluation
- Feature Importance

**Development Environment**
- Jupyter Notebook

---

## 📂 Project Files

- 📓 [Jupyter Notebook](./Power_Consumption_Prediction.ipynb)
- 📊 [PowerPoint Presentation](./Power_Consumption_Prediction.pptx)
- 📁 [Dataset](./dataset/powerconsumption.csv)

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

Data Analysis
Data Cleaning
Exploratory Data Analysis
Data Visualization
Feature Engineering
Machine Learning
Regression
Model Evaluation
Feature Importance
Python
Pandas
NumPy
Scikit-learn

👩‍💻 Author
Ramjot Kaur
Aspiring Data Analyst with hands-on experience in:
Python | SQL | Excel | Tableau | Power BI | Machine Learning | Data Visualization
🔗 Connect With Me
💼 LinkedIn – Ramjot Kaur
