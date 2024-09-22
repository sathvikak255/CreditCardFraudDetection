# Codtech-Task1

Name: Sathvika K
Company Name: Codtech IT Solutions
Domain: Machine Learning
Internship task: Credit Card Fraud Detection using a Machine Learning Model


# Credit Card Fraud Detection

## Project Overview

This project focuses on developing a machine learning model to detect fraudulent credit card transactions. Credit card fraud is a significant issue that affects consumers and financial institutions alike, and timely detection is crucial for minimizing losses.

### Objectives

- To create a robust model capable of identifying fraudulent transactions using various machine learning techniques.
- To address the challenges posed by imbalanced datasets, which are common in fraud detection scenarios.
- To evaluate model performance using appropriate metrics and ensure high recall for detecting fraud cases.

### Dataset

The dataset used for this project is sourced from Kaggle and contains transactions made by credit cards in September 2013 by European cardholders. It includes features such as:

- Transaction amounts
- Time of transaction
- Various anonymized features resulting from a PCA transformation

The target variable indicates whether a transaction is fraudulent (1) or not (0).

### Methodology

1. **Data Preprocessing:**
   - Load and explore the dataset.
   - Handle missing values (if any).
   - Scale features using StandardScaler for better model performance.

2. **Train-Test Split:**
   - Split the dataset into training and testing sets, ensuring stratification based on the target variable.

3. **Addressing Class Imbalance:**
   - Utilize SMOTE (Synthetic Minority Over-sampling Technique) to create synthetic examples of the minority class (fraudulent transactions) to balance the dataset.

4. **Model Development:**
   - Train an XGBoost classifier, known for its effectiveness in handling classification problems and large datasets.

5. **Evaluation:**
   - Evaluate the model using confusion matrix, classification report, and ROC-AUC score to understand performance metrics such as precision, recall, and F1-score.

### Technologies Used

- Python
- Libraries: pandas, numpy, scikit-learn, xgboost, imbalanced-learn, matplotlib, seaborn

### Results

The model achieved satisfactory results in detecting fraudulent transactions, with a focus on minimizing false negatives to ensure that fraud cases are identified effectively.

### Future Work

- Experiment with additional models and hyperparameter tuning to further improve performance.
- Implement a real-time fraud detection system for practical applications.
- Explore feature importance analysis to understand the key drivers of fraudulent behavior.
