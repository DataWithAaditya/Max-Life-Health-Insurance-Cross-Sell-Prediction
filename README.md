# Max-Life-Health-Insurance-Cross-Sell-Prediction

Project Overview
This project aims to predict whether an existing health insurance customer will be interested in purchasing an additional insurance policy. Using Machine Learning, we analyze customer data and identify key factors influencing cross-sell opportunities.

Dataset
- The dataset contains customer details, policy information, and past behavior.
- Features include age, region, vehicle details, policy sales channels, and past interactions.

Project Steps:
1. Data Wrangling & Cleaning – Handled missing values, outliers, and inconsistencies.
2. Feature Engineering – Selected and transformed relevant features.
3. Data Scaling & Handling Imbalance – Standardized numerical features and used SMOTE to balance the dataset.
4. Model Selection & Training – Compared multiple models (Logistic Regression, XGBoost, Random Forest) and optimized hyperparameters.
5. Model Evaluation – Used metrics like Accuracy, Precision, Recall, F1-Score, and AUC-ROC to assess performance.
6. Model Explainability – Applied SHAP to understand feature importance.

Final Model & Results:
- XGBoost provided the best balance between performance and interpretability after testing multiple models.
- Key insights: Age, Policy Sales Channel, Region Code, Vehicle Damage.
- Final accuracy: 0.8774
