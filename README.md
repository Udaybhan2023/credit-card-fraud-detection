 💳 Credit Card Fraud Detection

A complete end-to-end machine learning pipeline for detecting fraudulent 
credit card transactions using classical ML models with imbalance handling, 
threshold tuning, and full evaluation metrics.

## 📊 Dataset
- 284,807 transactions | 492 fraud cases (0.17%)
- 28 PCA-anonymized features (V1–V28) + Time + Amount
- Source: [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

## 🏆 Results

| Model               | Precision | Recall | F1-Score | Accuracy |
|---------------------|-----------|--------|----------|----------|
| Logistic Regression | 5.4%      | 82.1%  | 10.2%    | 97.57%   |
| Random Forest       | **94.5%** | 72.6%  | **82.1%**| **99.95%**|
| XGBoost             | 88.9%     | 75.8%  | 81.8%    | 99.94%   |

> ✅ Best model: **Random Forest** — highest F1 and precision on fraud class.

## 🔧 Pipeline

- Exploratory data analysis & visualizations
- Duplicate removal & feature scaling
- Class imbalance handling (undersampling + `class_weight='balanced'`)
- Model training: Logistic Regression, Decision Tree, Random Forest, XGBoost
- Evaluation: ROC-AUC, PR-AUC, F1, MCC, confusion matrix
- Decision threshold tuning
- Feature importance analysis

## 🚀 Getting Started

```bash
git clone https://github.com/your-username/credit-card-fraud-detection.git
cd credit-card-fraud-detection
pip install -r requirements.txt
jupyter notebook credit_card_fraud_detection.ipynb
```
