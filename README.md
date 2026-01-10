# 🎓 Student Test Score Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Library](https://img.shields.io/badge/Library-XGBoost-red)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
This project focuses on predicting student test scores based on various demographic and academic factors. By analyzing student data, the goal is to build a regression model that can accurately forecast performance, helping educators identify students who might need extra support.

**Author:** Muhammad Atif

## 📂 Dataset
The dataset contains information about students' backgrounds and their test results.
- **Target Variable:** `Score` (Continuous numerical value).
- **Features:** Likely includes variables such as study hours, previous scores, and other demographic details (processed via categorical analysis).

## 🛠 Tech Stack
- **Language:** Python
- **Data Manipulation:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** - `scikit-learn` (Pipelines, Preprocessing, Model Selection)
  - `xgboost` (XGBRegressor)

## 📊 Project Workflow

### 1. Data Loading & Cleaning
- Loaded the training and testing datasets.
- Checked for **missing values** and **duplicate rows** to ensure data quality.
- Verified the shape and structure of the data.

### 2. Exploratory Data Analysis (EDA)
- **Target Analysis:** Visualized the distribution of test scores.
- **Categorical Analysis:** Explored how different categories (like school type or gender) impact the scores.
- **Correlation Checks:** Identified relationships between features.

### 3. Preprocessing Pipeline
Implemented a robust `sklearn.pipeline.Pipeline` to prevent data leakage:
- **Numerical Features:** Scaled using `StandardScaler` / `MinMaxScaler`.
- **Categorical Features:** Encoded using `OneHotEncoder`.
- **Column Transformer:** Applied these transformations automatically within the model pipeline.

### 4. Model Comparison
Several regression algorithms were tested using **Cross-Validation (K-Fold)** to find the best performer:
- **Linear Models:** `LinearRegression`, `Ridge`, `Lasso`
- **Ensemble Models:** `RandomForestRegressor`, `GradientBoostingRegressor`
- **Boosting:** `XGBRegressor`

### 5. Final Submission
- The best-performing model pipeline was selected.
- Predictions were generated on the test set.
- A `submission.csv` file was created for final evaluation.

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/student-test-prediction.git](https://github.com/your-username/student-test-prediction.git)
