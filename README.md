# 🛡️ Insurance Enrollment Prediction

This project predicts whether an employee will opt into a voluntary insurance program based on demographic and job-related data.

## 📁 Dataset

Synthetic dataset with ~10,000 employee records.

Features:
- Demographics: `age`, `gender`, `marital_status`, `region`
- Employment: `salary`, `employment_type`, `tenure_years`, `has_dependents`
- Target: `enrolled` (1 = opted in)

## 🚀 Models Used

- Logistic Regression
- Random Forest (Tuned)
- XGBoost (Tuned)

All models tracked and compared using **MLflow**.

## 📈 Evaluation Metrics

- **Accuracy**
- **F1 Score**

## 🛠️ How to Run
- Hit run all cells on jupyter notebook or google colab :)

### 1. Clone the repo
```bash
git clone https://github.com/your-username/insurance-enrollment-prediction.git
cd insurance-enrollment-prediction
