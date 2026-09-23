# ⚡ ML Task 4 – Household Energy Consumption Prediction

## 📌 Project Overview

This project focuses on predicting **household energy consumption** using **Polynomial Regression**.

The model uses household and energy-usage-related features to predict the total **energy consumption in kWh**.

The project is implemented using **Python** and **Scikit-learn** in Google Colab/Jupyter Notebook.

---

## 🎯 Objective

The main objectives of this project are:

* Analyze the household energy consumption dataset.
* Identify and handle missing values.
* Select relevant input features.
* Apply Polynomial Regression.
* Predict household energy consumption.
* Evaluate the model using regression metrics.
* Compare actual and predicted energy consumption.
* Visualize the model predictions.

---

## 📂 Dataset

The dataset used in this project is:

**Household Energy Consumption Dataset**

### Features Used

The following features are used as input variables:

| Feature                | Description                       |
| ---------------------- | --------------------------------- |
| `Household_Size`       | Number of people in the household |
| `Avg_Temperature_C`    | Average temperature in Celsius    |
| `Peak_Hours_Usage_kWh` | Energy usage during peak hours    |

### 🎯 Target Variable

**`Energy_Consumption_kWh`**

This is the total household energy consumption measured in **kilowatt-hours (kWh)**.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **Matplotlib**
* **Scikit-learn**
* **Google Colab / Jupyter Notebook**

---

## 🔄 Workflow

The project follows these steps:

1. Import the required Python libraries.
2. Load the CSV dataset.
3. Check the dataset shape.
4. Display the first few records.
5. Analyze dataset information and statistics.
6. Check for missing values.
7. Remove rows containing missing values.
8. Select input features and target variable.
9. Split the dataset into training and testing sets.
10. Generate polynomial features with degree 2.
11. Train a Linear Regression model using the polynomial features.
12. Make predictions on the test dataset.
13. Evaluate the model using regression metrics.
14. Display actual and predicted energy consumption.
15. Visualize actual vs predicted values.

---

## 🤖 Model Used

### Polynomial Regression

Polynomial Regression is used to model a non-linear relationship between the input features and household energy consumption.

In this project:

* **Polynomial Degree:** 2
* **Test Size:** 20%
* **Random State:** 42

Polynomial features are generated using:

```python
PolynomialFeatures(degree=2)
```

The transformed features are then provided to a **Linear Regression** model for training and prediction.

---

## 📊 Model Evaluation

The model performance is evaluated using the following metrics:

### 1. MAE – Mean Absolute Error

MAE measures the average absolute difference between the actual and predicted energy consumption values.

### 2. MSE – Mean Squared Error

MSE measures the average squared difference between the actual and predicted values. Larger errors have a greater effect on this metric.

### 3. RMSE – Root Mean Squared Error

RMSE is the square root of MSE and represents the prediction error in the same unit as the target variable, **kWh**.

### 4. R² Score

R² Score measures how well the model explains the variation in household energy consumption.

---

## 📈 Visualization

A scatter plot is created to compare:

* **Actual Energy Consumption**
* **Predicted Energy Consumption**

The visualization helps identify how closely the model's predictions follow the actual energy consumption values.

---

## 📋 Output

The notebook generates the following outputs:

* Dataset information
* Dataset shape
* First few dataset records
* Descriptive statistics
* Missing-value information
* Polynomial features
* Trained Polynomial Regression model
* MAE
* MSE
* RMSE
* R² Score
* Actual vs Predicted Energy Consumption table
* Actual vs Predicted scatter plot

---

## 📁 Project Structure

```text
ML_NTask_4/
│
├── ML_NTask_4.ipynb
├── household_energy_consumption.csv
└── README.md
```

---

## ✅ Conclusion

In this project, **Polynomial Regression** is applied to predict household energy consumption using **household size, average temperature, and peak-hours energy usage**.

The model is evaluated using **MAE, MSE, RMSE, and R² Score**. The actual and predicted energy consumption values are also compared using a scatter plot.

This project demonstrates how polynomial regression can be used to model relationships between multiple household-related factors and energy consumption.
