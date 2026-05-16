# Credit-Card-Risk-Analysis

This project focuses on detecting fraudulent credit card transactions using machine learning techniques. The objective is to accurately identify suspicious transactions while addressing the challenge of highly imbalanced financial data.

## 📂 Project Structure

```bash
├── creditcard.csv      # Dataset
├── main.ipynb          # Jupyter Notebook containing analysis and model training
└── README.md           # Project documentation
```

## 📊 Dataset

- Real-world anonymized credit card transaction dataset
- Features transformed using PCA for confidentiality
- Target variable:
  - `0` → Legitimate Transaction
  - `1` → Fraudulent Transaction
- Highly imbalanced dataset with very few fraud cases compared to normal transactions

## 🔑 Project Workflow

### Data Exploration

- Analyzed dataset structure, shape, and missing values
- Examined fraud vs legitimate transaction distribution
- Performed exploratory data analysis to identify fraud patterns
- Visualized feature correlations and transaction behavior
- Identified severe class imbalance in the dataset

### Data Preprocessing

- Normalized transaction amount features
- Performed train-test split for model evaluation
- Applied under-sampling to balance fraud and legitimate transaction classes

### Model Building

Implemented and compared machine learning models using Scikit-learn:

- Logistic Regression
- Random Forest

### Model Evaluation

Performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- PR-AUC Score
- Confusion Matrix
- Classification Report

Special focus was given to **Recall**, since missing fraudulent transactions is more costly than false alarms.

## 📈 Results

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC | PR-AUC |
|------|----------|-----------|--------|----------|---------|--------|
| Logistic Regression | 92.39% | 96.63% | 87.76% | 91.98% | 97.72% | 98.22% |
| Random Forest | 92.39% | 97.70% | 86.73% | 91.89% | 97.62% | 97.98% |

## ✅ Conclusion

Both models delivered strong fraud detection performance. Logistic Regression was selected as the preferred model due to its higher recall, making it more effective at identifying fraudulent transactions and reducing missed fraud cases in financial risk analysis.
