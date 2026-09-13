# Hospital-readmission-prediction
This project predicts whether a diabetic patient will be **readmitted within 30 days** using Logistic Regression with **L2 regularization**.

## Dataset

**UCI Diabetes 130-US Hospitals for Years 1999–2008**

The dataset contains patient demographic information, diagnosis codes, previous visits, medications, and clinical/laboratory-related variables.

## Methodology

* Data preprocessing using imputation
* Numerical feature scaling
* Categorical feature one-hot encoding
* 80/20 stratified train-test split
* Logistic Regression with L2 regularization
* Evaluation using ROC-AUC, precision, recall, and confusion matrix
* Threshold analysis to study false positives and false negatives

## Results

| Metric    | Result |
| --------- | -----: |
| ROC-AUC   | 0.6418 |
| Accuracy  | 88.84% |
| Precision | 50.00% |
| Recall    |  2.03% |

A lower classification threshold was also evaluated. At a threshold of **0.10**, recall increased to **63.80%**, reducing false negatives to **822**, while false positives increased to **7,983**.

## Conclusion

The model provides moderate discrimination. For a healthcare screening scenario, reducing **false negatives** can be more important than minimizing false positives. However, the final threshold should be determined using validated clinical and economic cost estimates in a real-world setting.

## Files

* `Hospital_readmission_prediction.ipynb` — Compl
