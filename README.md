# ML-assignment
# 🩸 Chronic Kidney Disease (CKD) Prediction
# 📌 Overview
This project uses supervised machine learning (Logistic Regression, KNN, Random Forest, Decision Tree) to predict Chronic Kidney Disease (CKD) from 24 clinical measurements. The primary objective is clinical safety—specifically minimizing False Negatives (missed diagnoses).

# Data Source
kaggle link : https://www.kaggle.com/datasets/mansoordaku/ckdisease

# Performance Summary
Due to the strong linear separability of the dataset after preprocessing, all models performed exceptionally well.

Random Forest (Best): 100% Accuracy, 0 False Negatives (Clinically Safest)

Decision Tree (Tuned): 97.5% Accuracy, 1 False Negative

Logistic Regression & KNN: 97.5% Accuracy, 2 False Negatives

# Data Pipeline
Preprocessing: Handled missing values via mean imputation, encoded categorical variables, and applied StandardScaler.

Validation: 80/20 train-test split using stratify=y. All imputation and scaling were strictly fitted on the training set to prevent data leakage.

# 💻 Tech Stack
Language: Python

Data Manipulation: Pandas, NumPy

Machine Learning: Scikit-Learn

Data Visualization: Matplotlib, Seaborn