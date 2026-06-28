# AI/ML Engineering Internship - DevelopersHub Corporation



##  Task: End-to-End ML Pipeline with Scikit-learn Pipeline API (Customer Churn Prediction)

###  Objective of Task
The primary objective of this task was to build a robust, clean, and reusable end-to-end machine learning pipeline using the Scikit-learn `Pipeline` and `ColumnTransformer` APIs. The business use-case focused on identifying structural churn risks within telecom subscriber data, ensuring the data transformation workflows are encapsulated perfectly to prevent data leakage during training and production scaling.

###  Methodology & Approach
1. **Data Ingestion & Integrity Setup:** Loaded the customer dataset using Pandas, separating standard feature sets from the target classification column (`Churn`).
2. **Advanced Pipeline Feature Engineering:** * **Numerical Pipeline:** Handled missing continuous boundaries and applied robust scaling protocols via `StandardScaler`.
   * **Categorical Pipeline:** Isolated multi-class and binary textual categorical data and transformed them smoothly using `OneHotEncoder(handle_unknown='ignore')`.
3. **Encapsulated Preprocessing:** Integrated both pipelines into a unified structural `ColumnTransformer` layout to guarantee automated preprocessing workflows.
4. **Model Architecture Design:** Constructed comprehensive estimation workflows joining the unified preprocessing engine directly with target estimators: **Logistic Regression** and **Random Forest Classifier**.
5. **Hyperparameter Optimization Loop:** Leveraged `GridSearchCV` accompanied by a 5-fold cross-validation (`cv=5`) structure to sweep through optimal algorithmic param grids (such as checking `n_estimators`, `max_depth` variations, and solver regulations).
6. **Production Serializing & Export:** Successfully serialized the ultimate optimal trained model architecture directly to disk using `joblib` for instant operational inference deployment.

###  Key Results & Observations
* **Zero Data Leakage:** By nesting data scalers and one-hot encoders directly inside Scikit-learn's structural `Pipeline` bounds, the risk of testing parameters blending into the training distribution was completely eliminated.
* **Algorithmic Evaluation:** The Random Forest architecture, when structurally tuned via cross-validation grid search loops, demonstrated deep capability over baseline linear models in establishing complex non-linear classification boundaries.
* **Production-Readiness Verified:** The successful file generation via `joblib.dump()` proved that the entire workflow—from raw textual/numerical feature scaling to final class determination—can now be dynamically loaded via an independent API service endpoint using a single line of code (`pipeline.predict()`).