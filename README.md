# Credit Risk Scorecard
### Predicting Loan Default Probability using Machine Learning
**Author:** Kayalvizhi S | M.S. FinTech, SRM Institute of Science and Technology

---

## Business Problem
Lenders face significant losses from borrowers who default on credit obligations.
Approving high-risk applicants increases bad debt; rejecting too many limits revenue.
This model helps lenders make smarter, data-driven approval decisions.

## Approach
- Dataset: 150,000 real borrower records (Give Me Some Credit - Kaggle)
- Handled class imbalance using SMOTE (only 6.7% defaulters)
- Trained XGBoost classifier with tuned decision threshold

## Results
| Metric | Score |
|--------|-------|
| AUC Score | 0.81 |
| Default Detection (Recall) | 54% |
| Overall Accuracy | 86% |

## Key Risk Factors Identified
1. Revolving credit utilization
2. Number of times 30-59 days past due
3. Debt ratio

## Tools Used
Python, XGBoost, Scikit-learn, SMOTE, Pandas, Matplotlib, Seaborn

## Business Interpretation
At a 0.45 threshold, the model flags high-risk applicants for manual review —
reducing expected credit losses while maintaining a competitive approval rate.
Threshold is tunable based on the lender's risk appetite.
