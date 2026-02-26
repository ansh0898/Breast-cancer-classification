Problem Statement:

Early detection of breast cancer significantly increases survival rates, but manual diagnosis based on multiple tumor characteristics can be complex and time-consuming.

The objective of this project is to develop a machine learning classification model that predicts whether a tumor is malignant or benign based on diagnostic measurements. The goal is to assist in early detection by improving prediction accuracy and reducing misclassification risk.






Project Overview


This project focuses on building a Breast Cancer Classification Model using Machine Learning techniques.

The main goal is to predict whether a tumor is Malignant (Cancerous) or Benign (Non-Cancerous) based on various medical features extracted from diagnostic measurements.

This project demonstrates the complete ML workflow — from data understanding and preprocessing to feature selection and model evaluation.

Project Workflow


1️ Data Loading

Loaded dataset using Pandas.

Checked dataset shape, structure, and summary statistics.

2️ Data Understanding

Used:

df.describe()

df.info()

Checked missing values

Checked duplicate values

This ensures the dataset is clean and ready for modeling.

3️ Exploratory Data Analysis (EDA)

Generated correlation matrix.

Identified strong and moderate relationships between features.

Correlation strength guide used:

|correlation| ≥ 0.7 → Strong relationship

0.5 ≤ |correlation| < 0.7 → Moderate relationship

0.3 ≤ |correlation| < 0.5 → Weak but usable

|correlation| < 0.3 → Less important

This helped in understanding which features influence the target variable the most.

4️ Feature Selection

Applied feature selection techniques:

SelectKBest (f_regression)

Recursive Feature Elimination (RFE)

This step helps:

Reduce dimensionality

Remove less important features

Improve model performance

Reduce overfitting

5️ Feature Scaling

Used MinMaxScaler to normalize feature values.

Scaling ensures:

All features are on the same range

Model performance improves

Faster convergence

6️ Model Building

Model used:

Decision Tree Classifier

Split dataset into:

Training set

Testing set

Using:

train_test_split()

7️ Model Evaluation

Evaluated model using:

Confusion Matrix

Classification Report

Accuracy Score

Metrics considered:

Accuracy

Precision

Recall

F1-Score

This helps in understanding:

How well the model predicts cancer cases

Whether it is missing malignant cases

Whether it is misclassifying benign cases


 Results

 

The model successfully classifies tumors as malignant or benign with good accuracy.

Decision Tree performed effectively due to:

Clear feature separability

Strong correlation among key tumor characteristics

 Key Learnings

Importance of EDA before modeling

How correlation helps in understanding relationships

Practical implementation of feature selection

Importance of scaling

Model evaluation beyond just accuracy


 Future Improvements
 

Try advanced models:

Random Forest

XGBoost

Logistic Regression

Perform cross-validation

Hyperparameter tuning

Compare multiple models


 Conclusion

This project demonstrates a complete end-to-end Machine Learning pipeline for a medical classification problem.

It highlights how structured data, proper preprocessing, and the right model selection can help build an effective predictive system.
