# Credit-Card-Risk-Analysis

This project focuses on detecting fraudulent credit card transactions using machine learning techniques. The goal is to identify suspicious transactions accurately while handling the challenge of highly imbalanced data.

## 📂 Project Structure

```bash
├── creditcard.csv      # Dataset
├── main.ipynb          # Jupyter Notebook
└── README.md           # Documentation
````

## 📊 Dataset

* Real-world anonymized credit card transaction dataset
* Features transformed using PCA for confidentiality
* Target variable:

  * `0` → Legitimate Transaction
  * `1` → Fraudulent Transaction
* Highly imbalanced dataset with very few fraud cases

## 🔑 Project Workflow

### Data Exploration

* Checked dataset structure and missing values
* Analyzed class distribution
* Visualized correlations between features
* Identified imbalance issues

### Data Preprocessing

* Feature scaling and normalization
* Train-test split
* Handling imbalanced data using SMOTE / resampling techniques

### Model Building

Implemented machine learning models such as:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost (optional)

### Model Evaluation

Performance evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Confusion Matrix
Special focus on **Recall** to minimize missed fraud transactions.

