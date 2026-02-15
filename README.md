Business Problem

The business problem is to predict customer churn (whether a customer will leave) using behavioral, demographic, and billing data. The goal is to proactively identify high-risk customers so the company can intervene with retention strategies before revenue is lost. The project builds and compares multiple machine learning models to determine the most accurate and actionable churn prediction approach.

Three Key Results

XGBoost achieved the strongest predictive performance (highest ROC-AUC on the test set), outperforming Logistic Regression, Random Forest, and Gradient Boosting. Short tenure, contract type (e.g., month-to-month), and payment method were among the most important churn drivers, based on feature importance analysis. Using a 0.40 probability threshold improved recall, allowing the business to capture more at-risk customers while maintaining balanced precision. How to Run the Code (3–6 Steps)

Place the dataset files (retentiondata_case.csv and retention_final_dataset.csv) in the same directory as the notebook. Open Group#7.Churn_Modeling_Clean.ipynb in Jupyter Notebook or JupyterLab. Run all cells sequentially from top to bottom to perform data cleaning, feature engineering, and visualization. The notebook automatically splits the data into training, test, and holdout sets. Model pipelines with cross-validation and hyperparameter tuning will execute and select the best-performing model. Review final evaluation metrics, confusion matrix, ROC curve, and feature importance outputs for interpretation. One Limitation / Risk to Note

The model performance depends on historical data patterns, meaning it may not generalize well if customer behavior changes (e.g., pricing updates, new competitors, policy shifts). Additionally, optimizing for higher recall (to catch more churners) may increase false positives, potentially leading to unnecessary retention costs.
