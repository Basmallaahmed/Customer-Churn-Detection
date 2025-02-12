🚀 Customer Churn Detection 📊
🌟 Introduction
Predicting customer churn is a crucial task for businesses to retain customers and reduce revenue loss. This project leverages historical customer data to build a machine learning model that predicts whether a customer is likely to churn (exit) or stay. These insights empower businesses to take proactive measures to retain at-risk customers.

📂 Dataset Overview
Source: Churn_Modelling.csv
Features:
CreditScore: Customer's credit score.
Geography: Customer location.
Gender: Gender of the customer.
Age: Customer's age.
Tenure: Number of years with the company.
Balance: Account balance.
NumOfProducts: Number of products the customer uses.
HasCrCard: Has a credit card (1 = Yes, 0 = No).
IsActiveMember: Active customer status (1 = Yes, 0 = No).
EstimatedSalary: Annual estimated salary.
Exited (Target): 1 = Churned, 0 = Retained.
🛠️ Steps of the Project
🔍 Loading the Dataset

Imported the dataset using pandas and performed exploratory analysis.
📊 Data Visualization

Visualized feature distributions (e.g., age, balance) and relationships between features using Matplotlib and Seaborn.
Generated a correlation heatmap to understand feature interactions.
🧹 Data Cleaning and Feature Engineering

Encoded categorical variables (e.g., Gender and Geography) using one-hot encoding.
Removed irrelevant columns (e.g., RowNumber, CustomerId, Surname).
📂 Data Splitting

Split the dataset into training (80%) and testing (20%) subsets.
⚖️ Handling Imbalanced Data

Applied SMOTE (Synthetic Minority Oversampling Technique) to balance the target variable.
📐 Feature Scaling

Standardized numerical features using StandardScaler to ensure consistency across algorithms.
🤖 Model Training and Evaluation

Trained four machine learning models:
K-Nearest Neighbors (KNN)
Naive Bayes
Support Vector Machine (SVM)
Decision Tree (DT)
Evaluated the models using:
Accuracy
Precision
Recall
F1-Score
ROC-AUC
🏆 Results and Insights

Compared the performance of all models and identified the best-performing one.
🎯 Results and Findings
🧠 Model	🎯 Accuracy	🔍 Precision	🔁 Recall	📊 F1-Score	📈 ROC-AUC
KNN	84%	82%	78%	80%	0.85
Naive Bayes	82%	80%	76%	78%	0.83
SVM	85%	83%	81%	82%	0.86
Decision Tree	88%	86%	85%	85%	0.89
✨ Key Insights
The Decision Tree model outperformed others with the highest accuracy and F1-score.
Balancing the dataset using SMOTE improved model performance significantly.
Visualization tools provided valuable insights into customer behavior and churn patterns.
📊 Visualizations
Feature Correlation Heatmap
Shows how features like Age, Balance, and Geography correlate with churn.
Target Distribution
Displays the class imbalance before and after applying SMOTE.
ROC Curve
Compares model performance using ROC-AUC scores.

9. **Results and Findings**  
   - Decision Tree provided the highest accuracy and F1-score, making it the best-performing model.

10. **Deployment and Conclusion**  
   - The trained Decision Tree model can now predict whether a customer is likely to churn or not.
