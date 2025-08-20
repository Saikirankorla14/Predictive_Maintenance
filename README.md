# Predictive_Maintenance

📌 Project Overview
This project aims to predict whether a machine will fail in the near future based on sensor readings. By predicting failures, maintenance can be scheduled proactively to avoid costly downtime. The project uses the AI4I 2020 Predictive Maintenance Dataset from Kaggle.
🎯 Business Problem
Unplanned machine failures lead to expensive downtime, production losses, and repair costs. The goal is to build a predictive model that: 
- Detects early signs of machine failure.
- Classifies the type of failure (Heat Dissipation, Power Failure, etc.).
- Provides interpretability so engineers know why a failure is predicted.
📂 Dataset
Dataset: AI4I 2020 Predictive Maintenance Dataset (Kaggle)

Key Features:
- Air temperature [K]
- Process temperature [K]
- Rotational speed [rpm]
- Torque [Nm]
- Tool wear [min]

Target:
- Failure Type (Multi-class: Heat Dissipation, Power Failure, etc.)
🛠️ Realistic Tasks
1. Imbalanced Data
Failures are rare in the dataset, which leads to class imbalance. Techniques such as SMOTE, class weighting, or anomaly detection approaches will be considered to address this issue.
2. Feature Engineering
Raw sensor readings may not be sufficient. New features will be created, such as:
- Rolling averages of Rotational Speed and Torque.
- Standard deviations over time windows.
- Interaction features between temperature and torque.
3. Interpretability
Engineers need explanations, not just predictions. SHAP values will be used to highlight which sensor features (e.g., high torque, abnormal speed) are contributing to the failure prediction.
4. Multi-Class Classification
The target variable has multiple failure types (e.g., Heat Dissipation, Power Failure). Models such as Random Forest, XGBoost, or Neural Networks will be trained and evaluated to classify different failure modes.
📌 Workflow
1. Data Preprocessing (cleaning, handling imbalance).
2. Feature Engineering (rolling stats, derived features).
3. Model Training (multi-class classification models).
4. Model Evaluation (accuracy, F1-score, confusion matrix).
5. Interpretability (SHAP analysis).
6. Deployment (dashboard or API for real-time predictions).
✅ Expected Outcomes
- Early warning system for machine failures.
- Reduced unplanned downtime and maintenance costs.
- Interpretability for engineers to trust predictions.
- Ability to classify different failure types with reasonable accuracy.
