# 💳 Credit Card Fraud Detection

## 📌 Project Overview

This project aims to develop a machine learning model to detect **fraudulent credit card transactions** with high accuracy and reliability. Credit card fraud is a growing concern for both consumers and financial institutions, making early and precise detection essential for minimizing financial losses and preventing abuse.

---

## 🎯 Objectives

- Develop a robust model capable of identifying fraudulent transactions.
- Address the **class imbalance** challenge typical in fraud detection datasets.
- Evaluate performance using meaningful metrics, with an emphasis on achieving high **recall** to avoid missing fraudulent cases.

---

## 📊 Dataset

- **Source:** [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- **Description:** Contains credit card transactions made by European cardholders in September 2013.
- **Features include:**
  - `Time` of transaction
  - `Amount` of transaction
  - 28 anonymized principal components (`V1` to `V28`) from PCA transformation
  - `Class` (Target): `1` = Fraudulent, `0` = Legitimate

---

## 🔍 Methodology

### 1. **Data Preprocessing**
- Load and inspect the dataset
- Check for and handle any missing values
- Normalize transaction amounts using `StandardScaler`

### 2. **Train-Test Split**
- Split the dataset into training and testing sets
- Use **stratification** to maintain class distribution

### 3. **Handling Imbalanced Data**
- Apply **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the classes by generating synthetic samples for the minority class

### 4. **Model Building**
- Train an **XGBoost Classifier**, known for its speed, performance, and handling of imbalanced data

### 5. **Model Evaluation**
- Use the following metrics to assess model performance:
  - **Confusion Matrix**
  - **Classification Report** (Precision, Recall, F1-score)
  - **ROC-AUC Score**

---

## 🧪 Technologies & Libraries

- **Language:** Python  
- **Libraries:**  
  - `pandas`, `numpy` – Data manipulation  
  - `scikit-learn` – Preprocessing, metrics, and model evaluation  
  - `xgboost` – Gradient boosting classifier  
  - `imbalanced-learn` – SMOTE  
  - `matplotlib`, `seaborn` – Data visualization

---

## ✅ Results

The model successfully detects a significant number of fraudulent transactions, with high **recall** and a balanced **precision-recall tradeoff**, minimizing false negatives to ensure fraud cases are effectively flagged.

---

## 🔮 Future Improvements

- Explore more advanced models (e.g., Random Forest, LightGBM, Neural Networks)
- Perform extensive **hyperparameter tuning** to enhance model performance
- Integrate the model into a **real-time fraud detection pipeline**
- Conduct **feature importance analysis** to identify key indicators of fraud

---

## 💻 Installation & Running Locally

To get this project running on your local machine, follow the steps below:

### 1. Clone the repository
```bash
git clone https://github.com/sathvikak255/CreditCardFraudDetection.git
cd CreditCardFraudDetection
```

### 2. Install dependencies
Ensure that you have Python 3.x installed, then install the required libraries:
```bash
pip install -r requirements.txt
```

### 3. Run the Jupyter Notebook
This project includes a Jupyter Notebook where the model is built and evaluated. You can run the notebook by using the following command:
```bash
jupyter notebook CreditCardFraudDetection.ipynb
```

---

## 🤝 Contributing

We welcome contributions! Feel free to fork the repository, create a new branch, and submit a pull request. Please make sure your code adheres to the style guide and passes all tests.

If you have suggestions or feedback, feel free to open an **issue**.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👥 Author

**Sathvika K**  
GitHub: [sathvikak255](https://github.com/sathvikak255)
