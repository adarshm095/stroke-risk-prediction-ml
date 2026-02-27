🧠 Stroke Risk Prediction using Machine Learning
📌 Overview

This project builds an end-to-end machine learning pipeline to predict the likelihood of stroke based on patient demographic and health-related attributes. The objective is to assist in early risk detection using data-driven decision support.

The project focuses on handling class imbalance, preventing data leakage, and optimizing recall to minimize false negatives in medical prediction.

🚀 Key Features

Complete ML pipeline from data preprocessing to evaluation

Stratified train-test split to preserve class distribution

Class imbalance handled using SMOTE

Multiple model comparison:

Logistic Regression

Decision Tree

K-Nearest Neighbors

Random Forest

Recall-focused model selection (medical priority)

ROC-AUC evaluation for model discrimination

Feature importance analysis for interpretability

🛠 Tech Stack

Python

Pandas & NumPy

Scikit-learn

Matplotlib & Seaborn

Imbalanced-learn (SMOTE)

📊 Dataset Description

The dataset includes patient information such as:

Age

Hypertension

Heart disease

Average glucose level

BMI

Smoking status

Work type

Residence type

Target variable:

0 → No Stroke

1 → Stroke

The dataset is highly imbalanced, making recall an important evaluation metric.

⚙️ Project Workflow

Data Cleaning

Removed unnecessary features (ID)

Handled missing BMI values

Encoded categorical variables

Data Preprocessing

Stratified train-test split

Feature scaling

SMOTE applied to training data

Model Building

Implemented 4 classification models

Compared performance metrics

Model Evaluation

Accuracy

Recall (priority metric)

Confusion Matrix

ROC-AUC Curve

Model Interpretation

Feature importance using Random Forest

📈 Results

High recall achieved for minority class detection

Random Forest performed best in balancing precision and recall

Key influential features identified for stroke prediction

This demonstrates the importance of recall-focused optimization in healthcare ML systems.

🧠 Key Learnings

Accuracy can be misleading in imbalanced datasets

Data leakage must be avoided by splitting before scaling

SMOTE significantly improves minority class detection

Recall is more critical than accuracy in medical risk prediction

🔮 Future Improvements

Hyperparameter tuning using GridSearchCV

Deployment using Streamlit

Integration with real-time healthcare data

Model explainability using SHAP