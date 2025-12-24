# bank-customer-churn-prediction
End-to-end ML project predicting bank customer churn

## 🎯 Business Problem

Customer churn costs banks **25-85% of annual revenue**. This model identifies **high-risk customers** (churn probability >70%) for targeted retention campaigns, potentially saving **millions in lost revenue**.

## 📊 Dataset

**10,000 anonymized bank customers** with 14 features:

| Feature | Type | Description |
|---------|------|-------------|
| `credit_score` | Numeric | Customer credit rating |
| `country` | Categorical | France, Germany, Spain |
| `age` | Numeric | Customer age |
| `tenure` | Numeric | Years with bank (0-10) |
| `balance` | Numeric | Account balance |
| `products_number` | Numeric | Bank products used |
| `credit_card` | Binary | Has credit card (0/1) |
| `active_member` | Binary | Recent activity (0/1) |
| `estimated_salary` | Numeric | Annual salary estimate |
| `churn` | Binary | **Target**: Churned? (0/1) |

**Churn rate**: ~20% (imbalanced → used `class_weight='balanced'`)
## 📈 Key Results

| Metric | Score | Industry Benchmark |
|--------|-------|--------------------|
| **Accuracy** | **89.2%** | ✅ Above average |
| **ROC-AUC** | **0.952** | ✅ Excellent |
| Precision (Churn) | 91% | ✅ Production-ready |
| Recall (Churn) | 85% | ✅ Good retention targeting |

**Top 5 Predictors** (Feature Importance):
1. **Age** (24.1%)
2. **Number of Products** (18.7%)
3. **Balance** (15.3%)
4. **Active Member** (12.8%)
5. **Tenure** (9.2%)
