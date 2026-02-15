Loan Default Prediction
📌 Overview

This project builds an end-to-end machine learning pipeline to predict whether a loan applicant will default. The objective is to help financial institutions identify high-risk borrowers and reduce credit risk.

The project emphasizes:

Data leakage prevention

Class imbalance handling

Proper evaluation beyond accuracy

📊 Dataset

148,670 loan records

Binary classification problem (Default / No Default)

Imbalanced target distribution

⚙️ Approach
1️⃣ Data Cleaning

Removed leakage features (ID, Security_Type, Secured_by, construction_type)

Handled missing values using imputation

One-hot encoded categorical variables

2️⃣ Model

Logistic Regression

StandardScaler for feature normalization

class_weight="balanced" to handle imbalance

3️⃣ Evaluation Metrics

Accuracy: 84%

Recall (Default class): 71%

Precision (Default class): 66%

F1-score (Default class): 0.68

ROC-AUC: 0.867

📈 Why Logistic Regression?

Tree-based models achieved unrealistic perfect accuracy due to structural separability in the dataset. Logistic Regression was selected to ensure robustness and prevent overfitting caused by leakage patterns.

🧠 Key Learnings

Importance of preventing data leakage

Handling imbalanced classification problems

Evaluating models using ROC-AUC and recall instead of accuracy alone

Building clean, reproducible ML pipelines

🚀 Tech Stack

Python

Pandas

NumPy

Scikit-learn

Matplotlib