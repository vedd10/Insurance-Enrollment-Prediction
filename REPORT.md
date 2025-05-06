# Insurance Enrollment Prediction Report

## 📊 Data Observations

- Dataset contains ~10,000 synthetic employee records with demographic and job-related features.
- Target variable `enrolled` is binary (1 for opted-in to insurance, 0 otherwise).
- No missing values.
- Slight class imbalance, but manageable.

## 🧠 Model Choices & Rationale

- **Logistic Regression**: Used as a baseline model. Simple and interpretable.
- **Random Forest**: Good for capturing non-linearities and interactions. Tuned using RandomizedSearchCV.
- **XGBoost**: Powerful gradient boosting model, typically performs well on tabular data. Also tuned.

## 📈 Evaluation Results

| Model                 | Accuracy | F1 Score |
|--------------------   |----------|----------|
| Logistic Regression   | ~0.79    |  ~0.83   |
| Random Forest (tuned) | ~0.84    |  ~0.87   |
| XGBoost (tuned)       | ~0.99    |  ~0.99   |

> XGBoost performed best on both accuracy and F1-score.

## 🔍 Feature Importance (XGBoost)

Top features (based on model importance):

- Salary
- Age
- Tenure (years)
- Employment Type
- Has Dependents

## 📝 Key Takeaways

- Tree-based models outperform Logistic Regression.
- Income, age, and job-related characteristics are strong predictors of insurance opt-in.
- MLflow was used for experiment tracking and model comparison.

## 🚀 Next Steps

- Cross-validation for more robust evaluation.
- Expose the model through an API (e.g., FastAPI).
- Add automated CI/CD testing or cloud deployment.

