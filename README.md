# Customer-Churn-Detection
## **Steps of the Project**
1. **Loading the Dataset**  
   - The dataset `Churn_Modelling.csv` was loaded using pandas. It contains customer demographics, financial behavior, and service engagement data.

2. **Data Exploration and Cleaning**  
   - Inspected the dataset for missing or inconsistent values.  
   - Performed initial data exploration to understand feature distributions and relationships.

3. **Data Visualization**  
   - Used Matplotlib and Seaborn to visualize:  
     - Distribution of numerical features (e.g., Age, Balance).  
     - Relationship between categorical features (e.g., Gender, Geography) and churn.  
     - A heatmap to visualize feature correlations.  

4. **Feature Engineering**  
   - Encoded categorical variables such as `Gender` and `Geography` using one-hot encoding.  
   - Dropped irrelevant columns (`RowNumber`, `CustomerId`, `Surname`) to avoid bias.

5. **Data Splitting**  
   - Split the dataset into training (80%) and testing (20%) sets.

6. **Oversampling for Imbalanced Dataset**  
   - Applied the Synthetic Minority Oversampling Technique (SMOTE) to balance the dataset.

7. **Feature Scaling**  
   - Standardized numerical features to ensure uniform scaling using `StandardScaler`.

8. **Model Training and Evaluation**  
   - Trained and evaluated four machine learning algorithms:
     - K-Nearest Neighbors (KNN)
     - Naive Bayes
     - Support Vector Machine (SVM)
     - Decision Tree (DT)
   - Compared the models based on metrics such as accuracy, precision, recall, F1-score, and ROC-AUC.

9. **Results and Findings**  
   - Decision Tree provided the highest accuracy and F1-score, making it the best-performing model.

10. **Deployment and Conclusion**  
   - The trained Decision Tree model can now predict whether a customer is likely to churn or not.
