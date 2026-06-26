# Heart Disease Prediction System

A machine learning classification pipeline designed to predict the probability of heart disease using structured patient clinical data and diagnostic metrics.

## 🚀 Project Overview
This repository contains a robust diagnostic tool that applies machine learning algorithms to identify potential heart disease risks early. By utilizing multi-parameter medical data, the project benchmarks advanced classification models to balance diagnostic sensitivity and specificity, providing clinical decision-making insights.

## 📊 Dataset & Key Features
The pipeline is designed around structured clinical data from the UCI ML Repository, featuring a clean dataset with **zero missing values**. It utilizes the following exact features:

*   **Demographics**: `age`, `sex`
*   **Vital Signs**: `resting blood pressure`, `max heart rate`
*   **Diagnostic Markers**: `serum cholestoral`, `fasting blood sugar`, `resting electrocardiographic results`
*   **Clinical Status**: `chest pain type`, `exercise induced angina`, `oldpeak`, `ST segment`, `major vessels`, `thal`
*   **Target Variable**: `heart disease` (0 = Negative, 1 = Positive)

## 📊 Model Performance Benchmark

Here is the empirical performance summary across all benchmarked models:

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression** | **0.8519** | **0.8551** | **0.8519** | **0.8483** |
| **Support Vector Machine (SVM)** | 0.7963 | 0.7949 | 0.7963 | 0.7953 |
| **Random Forest** | 0.7593 | 0.7580 | 0.7593 | 0.7515 |
| **XGBoost** | 0.7593 | 0.7562 | 0.7593 | 0.7552 |

### 🔍 Key Insights:
*   **Best Performer**: **Logistic Regression** outperformed all other models across every metric, reaching an overall **Accuracy of 85.19%** and a balanced **Recall of 85.19%**. 
*   **Why Logistic Regression Won**: In clinical datasets with a relatively small sample size and direct correlation between markers (like chest pain and max heart rate) and heart disease, simpler linear models often generalize better and avoid the overfitting that complex ensemble methods (like Random Forest or XGBoost) experience.

## 🛠️ Tech Stack
*   **Language**: Python 3.x
*   **Machine Learning**: Scikit-Learn, XGBoost
*   **Data Libraries**: Pandas, NumPy
*   **Visualization**: Matplotlib, Seaborn

