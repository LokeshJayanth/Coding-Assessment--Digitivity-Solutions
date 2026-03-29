# Coding Assessment – Digitivity Solutions

This repository contains my submission for the **Digitivity Solutions Coding Assessment**.

## 📌 Project Title
**Student Performance Prediction using Machine Learning**

## 📖 Project Overview
The objective of this project is to analyze student performance data and build a machine learning model to predict whether a student is likely to **Pass or Fail** based on demographic and educational background factors.

This project demonstrates the complete **Data Science workflow**, including:
- data loading
- data cleaning
- exploratory data analysis (EDA)
- visualization
- feature engineering
- model training
- evaluation

---

## 📂 Dataset Information
The dataset used in this project contains the following features:

- `gender`
- `race/ethnicity`
- `parental level of education`
- `lunch`
- `test preparation course`
- `math score`
- `reading score`
- `writing score`

A new feature called **`average_score`** was created using the three subject scores, and based on that, students were classified into:

- **Pass (1)** → average score ≥ 50
- **Fail (0)** → average score < 50

---

## ⚙️ Steps Performed

### 1. Data Loading
The dataset was loaded using **Pandas**.

### 2. Data Cleaning
- Checked for missing values
- Handled missing values (if any)

### 3. Feature Engineering
- Created `average_score`
- Created target column `Result`

### 4. Exploratory Data Analysis (EDA)
Performed analysis to understand:
- score distribution
- student category patterns
- feature relationships

### 5. Data Visualization
Created multiple visualizations such as:
- Pass vs Fail chart
- Gender vs Average Score
- Test Preparation vs Average Score
- Correlation Heatmap
- Confusion Matrix
- Feature Importance

### 6. Model Building
Used **Random Forest Classifier** to build the prediction model.

### 7. Model Evaluation
Evaluated the model using:
- Accuracy Score
- Classification Report
- Confusion Matrix

---

## 🧠 Machine Learning Model Used
- **Random Forest Classifier**

To improve handling of class imbalance, the model was trained using:

```python
RandomForestClassifier(class_weight='balanced', random_state=42)
