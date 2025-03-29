# 🏢 Employee Attrition Prediction using Logistic Regression

## 📌 Overview

This project implements **Logistic Regression** to predict employee attrition based on HR data. It follows a structured **machine learning pipeline**, including **data preprocessing, feature encoding, feature scaling, model training, evaluation, and feature engineering**. Additionally, **Polynomial Features** are used to enhance the model’s predictive power.

---

## 📂 Project Structure

- **EmployeeAttrition.ipynb** - Jupyter Notebook with the complete model implementation.
- **HR_comma_sep.csv** - Dataset used for training and testing.
- **README.md** - Documentation for the project.

---

## 🛠 Approach

### 1️⃣ Data Preprocessing
- Load the **HR Employee Dataset**.
- Check for missing values and outliers.
- Convert categorical variables to numerical using **One-Hot Encoding**.
- Normalize features using **StandardScaler**.

### 2️⃣ Feature Engineering
- Remove less relevant features (`Work_accident`, `promotion_last_5years`) to improve efficiency.
- Apply **Polynomial Feature Transformation** to capture complex relationships between variables.

### 3️⃣ Model Implementation
- **Logistic Regression** is implemented using `sklearn.linear_model.LogisticRegression`.
- Data is split into **80% training** and **20% testing** using `train_test_split`.
- The model is optimized using **gradient descent**.

### 4️⃣ Model Evaluation
- Evaluate using:
  - **Accuracy**
  - **Precision, Recall, and F1-score**
  - **Confusion Matrix**
  - **Polynomial Feature Enhancement Analysis**
- Compare the standard logistic regression model with a **Polynomial Features model**.

### 5️⃣ Making Predictions
- Test the model on unseen employee data.
- Standardize new input features before prediction.
- Classify employees as **likely to leave (1) / stay (0)**.

---

## 📊 Dataset

The dataset used in this project is an **HR Employee Dataset** containing work-related attributes for employees.

### Dataset Features:
- **satisfaction_level** - Employee satisfaction level.
- **last_evaluation** - Last performance evaluation score.
- **number_project** - Number of projects handled.
- **average_montly_hours** - Average monthly working hours.
- **time_spend_company** - Number of years at the company.
- **Work_accident** - Whether the employee had a work accident (0/1).
- **left** - Target variable (1 = Employee left, 0 = Stayed).
- **promotion_last_5years** - Whether the employee was promoted in the last 5 years (0/1).
- **Department** - Department of the employee (Categorical).
- **salary** - Salary category (Low, Medium, High - Categorical).

---

## 🔧 Technologies Used

- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib & Seaborn**
- **Scikit-Learn** (Machine Learning)

---

## 📊 Performance Metrics

| Model | Accuracy |
|--------|----------|
| Logistic Regression | **75.07%** |
| Logistic Regression with Polynomial Features (Degree 3) | **92.73%** |

---

## 📥 Installation

Install dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
