# Rainfall-Prediction
**Course Title:** Machine Learning Lab 

**Course Code:** CSE-5211

**Author:** Sahbaj Bin Seraj, Sidratul Muntaha

**Supervised By:**  **Md. Mynoddin**

Assistant Processor, Department of CSE, Rangamati Science and Technology University.
# Rainfall Prediction Using Machine Learning
## 1. Introduction

**1.1 Problem Statement:** Rainfall prediction is essential for agriculture, disaster management, and water resource planning. Traditional methods often lack accuracy due to complex weather patterns.

**1.2 Objective:** To apply machine learning models for more accurate rainfall prediction.

**1.3 Machine Learning Approaches Used:** Logistic Regression, Support Vector Classifier (SVC), and XGBoost.

**1.4 Tools Used:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn.

## 2. Methodology

### 2.1 Data Overview
**Dataset Shape:** 366 rows, 12 columns.

**Features:** Day, pressure, max temperature, temperature, min temperature, dew point, humidity, cloud, rainfall, sunshine, wind direction, wind speed.

**Target Variable:** Rainfall (Yes/No).

### 2.2 Data Preprocessing

**Dataset:** Includes meteorological parameters like temperature, humidity, and wind speed.

**Handling Missing Values:** Mean imputation was applied.

**Categorical Encoding:** Yes/No values were converted to binary (1/0).

**Feature Scaling:** StandardScaler was used to normalize data.

### 2.3 Feature Selection & Handling Class Imbalance

Highly correlated features (e.g., maxtemp and mintemp) were removed to avoid redundancy.

Random OverSampling was applied to balance the dataset.

### 2.4 Model Training & Evaluation

**Models Used:** Logistic Regression, SVC, XGBoost.

**Performance Metric:** Accuracy, Precision, Recall, F1-score.

**Validation Strategy:** Data split into 80% training and 20% validation.

## 3. Results

**Model** ---------------- **Precision** --- **Recall** --- **F1-Score** --- **Accuracy**

**Logistic Regression** ----- 0.82 ------ 0.83 ------ 0.82 ------- 0.89

**XGBoost Classifier** ------ 0.76 ------ 0.73 ------ 0.74 ------- 0.83

**SVC**	---------------------- 0.85 ------ 0.80 ------ 0.82 ------- 0.88

### 3.1 Key Observations:

The Logistic Regression model performed well with 89% accuracy.

**Classwise Statistics of Logistic Regression model**

**Model** -------- **Precision** --- **Recall** ---	**F1-Score** --- **Support**

Class 0	 ----------- 0.78	------- 0.75 ------ 0.77 -------- 24

Class 1 ----------- 0.88 ------- 0.90 ------ 0.89 -------- 50

## 4. Conclusion & Future Work

**Conclusion:** Machine learning models, especially Logistic Regression and SVC, significantly enhance rainfall prediction accuracy.

**Limitations:** Model struggles slightly with non-rain cases, leading to some false positives.

**Future Work:** Implementing deep learning techniques and optimizing feature selection to improve accuracy further.

## 5. References
[1] Dataset Source: [https://www.geeksforgeeks.org/rainfall-prediction-using-machine-learning-python/]
