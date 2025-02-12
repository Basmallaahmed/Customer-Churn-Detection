# 🚀 Customer Churn Detection 📊

## 🌟 Introduction
Predicting customer churn is a crucial task for businesses to retain customers and reduce revenue loss. This project leverages historical customer data to build a machine learning model that predicts whether a customer is likely to churn (exit) or stay. These insights empower businesses to take proactive measures to retain at-risk customers.

---

## 📂 Dataset Overview
- **Source**: `Churn_Modelling.csv`
- **Features**:
  - **CreditScore**: Customer's credit score.
  - **Geography**: Customer location.
  - **Gender**: Gender of the customer.
  - **Age**: Customer's age.
  - **Tenure**: Number of years with the company.
  - **Balance**: Account balance.
  - **NumOfProducts**: Number of products the customer uses.
  - **HasCrCard**: Has a credit card (1 = Yes, 0 = No).
  - **IsActiveMember**: Active customer status (1 = Yes, 0 = No).
  - **EstimatedSalary**: Annual estimated salary.
  - **Exited** (Target): 1 = Churned, 0 = Retained.

---

## 🛠️ Steps of the Project

1. **🔍 Loading the Dataset**
   - Imported the dataset using pandas and performed exploratory analysis.

2. **📊 Data Visualization**
   - Visualized feature distributions (e.g., age, balance) and relationships between features using Matplotlib and Seaborn.
   - Generated a correlation heatmap to understand feature interactions.

3. **🧹 Data Cleaning and Feature Engineering**
   - Encoded categorical variables (e.g., `Gender` and `Geography`) using one-hot encoding.
   - Removed irrelevant columns (e.g., `RowNumber`, `CustomerId`, `Surname`).

4. **📂 Data Splitting**
   - Split the dataset into training (80%) and testing (20%) subsets.

5. **⚖️ Handling Imbalanced Data**
   - Applied SMOTE (Synthetic Minority Oversampling Technique) to balance the target variable.

6. **📐 Feature Scaling**
   - Standardized numerical features using `StandardScaler` to ensure consistency across algorithms.

7. **🤖 Model Training and Evaluation**
   - Trained four machine learning models:
     - **K-Nearest Neighbors (KNN)**
     - **Naive Bayes**
     - **Support Vector Machine (SVM)**
     - **Decision Tree (DT)**
   - Evaluated the models using:
     - **Accuracy**
     - **Precision**
     - **Recall**
     - **F1-Score**
     - **ROC-AUC**

8. **🏆 Results and Insights**
   - Compared the performance of all models and identified the best-performing one.

---

## 🎯 Results and Findings

| 🧠 **Model**         | 🎯 **Accuracy** | 🔍 **Precision** | 🔁 **Recall** | 📊 **F1-Score** | 📈 **ROC-AUC** |
|-----------------------|----------------|------------------|---------------|-----------------|----------------|
| **KNN**              | 77.85%         | 46.60%           | 60.69%        | 52.72%          | 0.7754         |
| **Naive Bayes**       | 75.40%         | 42.20%           | 56.51%        | 48.31%          | 0.7641         |
| **SVM**              | 80.85%         | 52.42%           | 63.63%        | 57.94%          | 0.8390         |
| **Decision Tree**     | 74.40%         | 40.80%           | 57.24%        | 47.64%          | 0.6801         |

### ✨ Key Insights
- **SVM** achieved the best performance overall, with the highest **Accuracy (80.85%)**, **F1-Score (57.94%)**, and **ROC-AUC (0.839)**, making it the best choice among the models evaluated.
- While **KNN** performed decently with a good balance of metrics, it did not outperform SVM.
- The **Naive Bayes** and **Decision Tree** models exhibited lower performance compared to the other algorithms, which indicates they may not be the best fit for this dataset without further tuning or additional features.


---

## 📊 Visualizations
1. **Feature Correlation Heatmap**  
   - Shows how features like `Age`, `Balance`, and `Geography` correlate with churn.
2. **Target Distribution**  
   - Displays the class imbalance before and after applying SMOTE.
3. **ROC Curve**  
   - Compares model performance using ROC-AUC scores.

---


