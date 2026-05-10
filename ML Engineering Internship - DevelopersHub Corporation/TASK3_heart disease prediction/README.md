 **Task 3: Heart Disease Prediction**

**Project Objective**
The goal of this project is to develop a machine learning model capable of predicting whether a person is at risk of heart disease based on their clinical and health data. This tool can assist in early diagnosis and preventive healthcare.

**Dataset Used**

- **Source:** Heart Disease UCI Dataset (Kaggle).
- **Features:** The dataset includes patient attributes such as age, sex, chest pain type, blood pressure, cholesterol, fasting blood sugar, and more.
- **Pre-processing:**

  - Handled missing values by dropping columns with low data density (`ca`, `thal`, `slope`).
  - Filled remaining null values using Mean (for numeric) and Mode (for categorical) values.
  - Applied One-Hot Encoding for categorical features to prepare the data for the model.

**Models Applied**

- **Algorithm:** Logistic Regression.
- **Approach:** - Split the data into 80% Training and 20% Testing sets.
  - Configured the model with `max_iter=1000` to ensure proper convergence during training.

**Key Results and Findings**

- **Accuracy:** The model achieved a solid accuracy of approximately **81.5%** on the test data.

 **Performance Evaluation:**
 
 - **Confusion Matrix:** Successfully identified true positive and true negative cases.
  - **ROC Curve:** The AUC score indicates strong predictive power and a good balance between sensitivity and specificity.
- **Top Predictors:** The analysis revealed that factors like **Exercise-induced Angina**, **Gender**, and **Regional health data** (dataset origin) are significant indicators of heart disease risk.

**Feature Importance**

Extracted coefficients from the Logistic Regression model to highlight the most significant predictors of heart disease, such as exercise-induced angina, specific dataset origins, and gender.
