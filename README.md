# 📊 Telco Customer Churn Analysis — EDA & Regression Modelling

## 📝 Project Overview

This project is submitted as part of the **FBS Data Cohort 1 Final Assessment**. It focuses on analysing the **Telco Customer Churn** dataset using Python. The project includes:

- Data Cleaning & Preprocessing  
- Exploratory Data Analysis (EDA)  
- Regression Modelling 

## 📁 Dataset

The dataset is sourced from [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn). It contains customer demographics, account details, and churn status.

## 1️⃣ Data Preprocessing

- Handled missing values in the `TotalCharges` column by converting it to a numeric type and dropping null rows.
- Checked data types and duplicates.
- Categorical variables were encoded, and numerical features scaled where appropriate.

## 2️⃣ Exploratory Data Analysis (EDA)

Key visualisations and findings include:

- **Churn Distribution**: The Majority of customers did not churn, but a significant portion did.
- **Correlation Heatmap**: `MonthlyCharges`, `TotalCharges`, and `tenure` showed relationships with churn and customer value.
- Insights suggest that long-tenured and bundled service customers are less likely to churn.

<img width="614" height="534" alt="correlation_tel" src="https://github.com/user-attachments/assets/9d1c91db-a9f6-4e84-83b8-9e04096c8981" />
 
<img width="515" height="411" alt="churn" src="https://github.com/user-attachments/assets/e0f95b6c-caec-4067-aca2-ea5493d7e65a" />


## 3️⃣ Regression Modelling

Regression was used to predict **Monthly Charges**, a proxy for customer value, using features like:

- Tenure
- Total Charges
- Contract Type
- Internet Service

### Models Used

- **Linear Regression**

### Evaluation Metrics

| Model                   | R² Score | RMSE   |
|------------------------|----------|--------|
| Linear Regression       | 0.8105448711897016 | 0.43012066861280623 |



## 🛠 Requirements

Install required libraries with:

```bash
pip install -r requirements.txt
```

## 🚀 Future Work
- Add a classification model to predict churn directly.

- Perform clustering to uncover customer segments.

- Deploy the model using a web app or API.
