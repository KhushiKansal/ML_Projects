### **Bank Marketing Lead Conversion Prediction**



* **Overview**

This project predicts whether a client will subscribe to a term deposit after a phone marketing campaign using machine learning techniques. The dataset is sourced from Kaggle.



* **Setup Instructions**

1\. Install the required Python libraries:

&nbsp;  pip install pandas numpy scikit-learn matplotlib seaborn



2\. Place the dataset file (Bank\_Marketing\_Original\_Data.csv) in your working directory.



3\. Open and run the Prediction\_of\_deposits.ipynb notebook.



\## Half-Page Project Summary



* **Objective:**

Predict whether a client will subscribe to a term deposit based on personal and campaign-related attributes.



* **EDA Insights:**

\- The target variable is imbalanced with more 'no' than 'yes'.

\- Features 'age' and 'job' showed notable relationships with the target:

&nbsp; - Older clients and retirees showed higher subscription rates.

&nbsp; - Clients in management roles had better conversion rates.



* **Baseline Model:**

A Logistic Regression model was trained as a baseline. It achieved reasonable accuracy and F1-score but was affected by class imbalance.



* **Improvement Attempt:**

A Random Forest Classifier with hyperparameter tuning via GridSearchCV was implemented to improve performance. The parameters tuned were:

\- Number of estimators (n\_estimators)

\- Maximum depth (max\_depth)

\- Minimum samples split (min\_samples\_split)



This improved the model’s performance, achieving an **AUC of 0.93.**



* **Final Results**



Metric               | Logistic Regression | Random Forest

---------------------|---------------------|---------------

Accuracy             | Moderate            | Improved

F1 Score             | Moderate            | Improved

ROC AUC              | Moderate            | 0.93



