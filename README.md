# 📈 Telecom Customer Churn Prediction

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/project-guided%20learning-informational)]()

This guided machine learning project focuses on predicting customer churn in the telecom industry using the **Telco Customer Churn** dataset. It was completed as part of a learning journey to strengthen skills in Python-based data science workflows — from data preprocessing and EDA to training and evaluating predictive models.

> ⚠️ **Note:** This is a guided project and not original work. It is included in my portfolio to demonstrate proficiency in core data science and machine learning techniques.

---

## 📚 Table of Contents

- [📂 Dataset](#-dataset)
- [🔍 Project Workflow](#-project-workflow)
- [📊 Technologies Used](#-technologies-used)
- [🚀 Future Improvements](#-future-improvements)
- [🎓 About This Project](#-about-this-project)

---

## 📂 Dataset

- **Source**: [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Records**: 7,043  
- **Features**: 21 (demographics, services, billing info, churn label)

Key attributes include:
- **Demographics**: `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- **Services**: `PhoneService`, `InternetService`, `TechSupport`, `StreamingTV`
- **Billing**: `Contract`, `PaymentMethod`, `MonthlyCharges`, `TotalCharges`
- **Target**: `Churn` (Yes/No)

---

## 🔍 Project Workflow

### 📌 1. Data Preprocessing
- Converted `TotalCharges` from object to numeric and handled missing values.
- Removed customer IDs for modeling.
- Applied label encoding for binary categories and one-hot encoding for multi-class features.
- Split dataset into training and test sets (80/20 split).
- Used `StandardScaler` to normalize numerical features.

### 📊 2. Exploratory Data Analysis (EDA)
Key insights:
- **Churn rate**: ~26.6% of customers churned.
- **Contract type**: Customers with month-to-month contracts churn significantly more.
- **Tenure**: Newer customers are more likely to churn.
- **Payment method**: Electronic check users had higher churn rates.
- **Internet service**: Fiber optic users showed higher churn.

Visualizations included:
- Count plots, histograms, box plots, and a correlation heatmap.

---

## 🤖 3. Machine Learning Model Evaluations and Predictions

### ✅ Models Trained:
- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Support Vector Classifier (SVC)  
- Decision Tree Classifier  
- Random Forest Classifier  
- AdaBoost Classifier  
- Gradient Boosting Classifier  
- Voting Classifier (ensemble of Logistic Regression, KNN, and Random Forest)

### 🧪 Evaluation Metrics:
All models were evaluated on:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **ROC AUC Score**
- **Confusion Matrix**

### 📊 Performance Comparison (Sample)

| Model                   | Accuracy | Precision | Recall | F1 Score | ROC AUC |
|------------------------|----------|-----------|--------|----------|---------|
| Logistic Regression    | 0.80     | 0.73      | 0.56   | 0.63     | 0.83    |
| K-Nearest Neighbors    | 0.77     | 0.70      | 0.50   | 0.58     | 0.79    |
| SVC                    | 0.79     | 0.74      | 0.54   | 0.62     | 0.82    |
| Decision Tree          | 0.74     | 0.63      | 0.60   | 0.62     | 0.73    |
| Random Forest          | 0.80     | 0.73      | 0.59   | 0.65     | 0.83    |
| AdaBoost               | 0.80     | 0.72      | 0.60   | 0.66     | 0.83    |
| **Gradient Boosting**  | **0.81** | **0.74**  | **0.63**| **0.68** | **0.84**|
| Voting Classifier      | 0.80     | 0.73      | 0.59   | 0.65     | 0.83    |

> 🥇 **Best Performer**: The Gradient Boosting Classifier showed the best overall performance, balancing accuracy and recall with the highest ROC AUC score.

---

## 📊 Technologies Used

- **Language**: Python 3.8+  
- **Tools**: Jupyter Notebook  
- **Libraries**:  
  - `pandas`, `numpy` – data manipulation  
  - `matplotlib`, `seaborn` – visualization  
  - `scikit-learn` – modeling and evaluation

---

## 🚀 Future Improvements

- Hyperparameter tuning using GridSearchCV or RandomizedSearchCV  
- Use of more advanced ensemble models like XGBoost or LightGBM  
- Model interpretability with SHAP or LIME  
- Deployment via Streamlit or Flask  
- Integration of customer feedback data or call logs

---

## 🎓 About This Project

This project was completed as part of a guided learning experience to practice machine learning concepts in Python. It helped me gain hands-on experience with:
- Data preprocessing
- EDA and visual storytelling
- Supervised classification models
- Model evaluation and comparison

---


