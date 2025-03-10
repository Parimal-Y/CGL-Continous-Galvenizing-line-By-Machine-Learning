Problem Statement
The Continuous Galvanizing Line (CGL) plays a critical role in steel manufacturing by applying a protective zinc coating to steel sheets. However, inconsistencies in coating weight, material hardness, and process parameters can lead to:
⚠️ Defects in steel sheets, affecting product quality.
⚠️ Inefficient use of raw materials, increasing production costs.
⚠️ Unexpected equipment failures, leading to downtime.

This ML model aims to provide data-driven insights to optimize the CGL process, reducing errors and improving efficiency.

Dataset Information
Source: Industrial data from a steel manufacturing CGL production line.
Features Include:
Process Parameters: Line speed, furnace temperature, pressure, air knife position, etc.
Material Properties: Coating weight, hardness, thickness, tensile strength, etc.
Quality Control Data: Defect detection logs, real-time sensor readings.
Preprocessing Steps:
✅ Handling Missing Values (Imputation, Mean/Median Filling).
✅ Feature Scaling (Standardization & Normalization).
✅ Feature Selection (Eliminating low-impact variables).
✅ Outlier Detection (Using IQR & Z-Score methods).

Technologies & Tools Used
Programming Language: Python 
Data Processing: Pandas, NumPy
Machine Learning Libraries:
Scikit-Learn (Random Forest, MultiOutputRegressor)
XGBoost (Boosted Decision Trees for regression tasks)
Data Visualization: Matplotlib, Seaborn
Model Deployment: (Planned for Flask, FastAPI, or Streamlit)
Model Persistence: Joblib (Saving trained models for future use)

Machine Learning Approach
This project uses supervised learning regression models to predict multiple output variables.

1️⃣ Model Selection & Training
Random Forest Regressor: Captures complex relationships between features.
XGBoost Regressor: Boosted decision trees for high accuracy.
MultiOutputRegressor: Handles multiple target variables simultaneously.
Train-Test Split: Dataset is split into 80% training & 20% testing.
2️⃣ Performance Evaluation
Mean Squared Error (MSE): Measures prediction error.
R² Score: Indicates how well the model explains variability in data.
Cross-Validation: 5-fold CV ensures robustness.
3️⃣ Model Optimization
Hyperparameter Tuning: Using GridSearchCV & RandomizedSearchCV.
Feature Importance Analysis: Identifying key factors influencing coating weight.
🚀 Results & Insights
✅ The model successfully predicts coating weight and hardness with high accuracy.
✅ Feature importance analysis highlights key parameters affecting final steel quality.
✅ Potential integration with real-time sensor data for live monitoring.

🔍 Key Observations
Air knife pressure & line speed significantly impact coating thickness.
Furnace temperature stability is crucial for maintaining consistent hardness.
Machine learning can reduce coating weight deviations, minimizing material waste.
