# 🩺 Breast Cancer Binary Classification


---

## 🧩 Project Overview
This project focuses on **predicting the nature of breast tumors**:

- **0 → Malignant (Cancerous)**  
- **1 → Benign (Non-Cancerous)**  

We implement and compare three classic machine learning models:

| Model | Library |
|-------|---------|
| Logistic Regression | ![Sklearn](https://img.shields.io/badge/scikit--learn-0.24-blue?logo=scikit-learn) |
| Support Vector Machine (SVM) | ![Sklearn](https://img.shields.io/badge/scikit--learn-0.24-blue?logo=scikit-learn) |
| K-Nearest Neighbors (KNN) | ![Sklearn](https://img.shields.io/badge/scikit--learn-0.24-blue?logo=scikit-learn) |

---

## 📊 Dataset Overview
**Breast Cancer Wisconsin (Diagnostic) Dataset** from scikit-learn:

- **Samples:** 569  
- **Features:** 30 numerical measurements  
- **Target classes:** 0 (Malignant), 1 (Benign)  
- **Data quality:** No missing values  


---

## 🏗 Methodology

### 1️⃣ Data Preparation
- Load dataset from `scikit-learn`  
- Split into **training (80%)** and **testing (20%)** sets using stratification  
- No feature scaling applied  

### 2️⃣ Model Training
Trained three models with default parameters:

- Logistic Regression  
- Support Vector Machine (SVM)  
- K-Nearest Neighbors (KNN)  

### 3️⃣ Model Evaluation
Metrics computed for each model:

| Metric | Description |
|--------|-------------|
| ✅ Accuracy | Overall correctness of predictions |
| 🎯 Precision | Correctness of positive predictions |
| 🩺 Recall | Ability to detect actual positives (critical for cancer detection) |
| ⚖️ F1-score | Harmonic mean of precision and recall |
| 📊 Confusion Matrix | Detailed breakdown of predictions |

---

## 📈 Model Comparison

| Model                  | Accuracy | Precision | Recall | F1-Score |
|------------------------|----------|-----------|--------|----------|
| Logistic Regression    | 0.96     | 0.95      | 0.98   | 0.97     |
| Support Vector Machine | 0.92     | 0.92      | 0.97   | 0.94     |
| K-Nearest Neighbors    | 0.91     | 0.94      | 0.91   | 0.92     |

> **Note:** Values may vary slightly depending on environment and dataset split.

---

## 🏅 Key Findings

- **Best Performing Model:** Logistic Regression (highest balance of accuracy & F1-score)  
- **Most Important Metric:** **Recall**, to minimize false negatives and ensure malignant tumors are not missed.  
- **Medical Implication:** High recall is critical for patient safety.  

---

## 📌 Conclusion
This project demonstrates how **classic ML models** can classify breast tumors effectively **without feature scaling**.  

- Logistic Regression achieved the best performance overall.  
- Recall is prioritized in healthcare applications to reduce misdiagnosis risks.  
- Proper train-test split, evaluation metrics, and model comparison were implemented.

---

## 📚 References
1. [Scikit-learn Breast Cancer Dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html)  
2. Tomczak, J. M. (2014). "Breast Cancer Wisconsin (Diagnostic) Data Set." UCI Machine Learning Repository.  
3. Brownlee, J. *Machine Learning Mastery*. "Classification Metrics for Imbalanced Data."

---

## 👨‍💻 Author
**Amjad fahad Al-thobaiti**  
