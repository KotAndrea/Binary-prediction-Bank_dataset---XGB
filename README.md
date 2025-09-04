#  Bank Term Deposit Prediction with XGBoost

This project is from a competition on Kaggle, where the goal is to predict whether a client will subscribe to a bank term deposit. I used XGBoost for binary classification and achieved a  relatively strong ROC AUC score.

##  Objective

Predict the probability that a client will subscribe to a term deposit based on various features in a synthetically generated banking dataset.

- **Target**: Binary variable `y` (1 = subscribed, 0 = not subscribed)
- **Evaluation Metric**: ROC AUC score

##  Dataset

- Synthetic dataset provided by Kaggle
- Train/test split handled by Kaggle competition format

> Note: The dataset files (`train.csv`, `test.csv`) are included in this repository under the `data/` folder. The notebook has been updated to use local paths, so you can run it directly without downloading anything from Kaggle.


##  Approach

- **Model**: XGBoost Classifier
- **Preprocessing**:
  - Label encoding 
  - Target encoding
  - feature engineering
- **Training**:
  - Optuna optimization with early stoppng condition
  - ROC AUC used for evaluation
- **Performance**:
  - Achieved private score: **0.96871**
