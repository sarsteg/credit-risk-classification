# Module 12 Report Template

## Overview of the Analysis

The **purpose** of the analysis is to train and evaluate a model on loan risk. The dataset used for the project is historical lending activity from a peer-to-peer lending services company. Variables in the dataset included loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status.

A logistic regression model will be used to identify the creditworthiness of borrowers as either **high-risk** (unhealthy loan/defaulting) or **low-risk** (healthy loan). 

To complete this project, I created two models. For each model, the dependent variable (y) was loan status. Loans are identified as either **defaulting** (1) or **healthy** (0). The remaining variables were used as predictors (x). Both models were based on samples of the data. Model 1 had an unbalanced distribution between the outcomes (defaulting vs healthy), so the second model adjusts for this by equalizing the sampling from each outcome. The models were first trained and then evaluated for their performance.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* **Machine Learning Model 1:**

  * Our **balanced accuracy score** is **95%**. The balanced accuracy score takes into account the sensitivity (true positive rate) and the specificity (true negative rate). The balanced accuracy score is measures the performance of our model, especially with imbalanced datasets. In our dataset, we have 75036 loans that were rejected, but only 2500 that were accepted. Since our data is imbalanced, the balanced accuracy score serves as a good metric for the performance of our model.
  * Another measure of performance for our model is **accuracy**. The model's accuracy score is **99%**, which means that the model correctly predicted 99% of all loans in the dataset.
  * Based on the **confusion matrix**, the model accurately accepted 18663 healthy loans and rejected 563 high-risk loans. However, the model also incorrectly rejected 102 healthy loans and incorrectly accepted 56 high-risk loans.
  * Precision looks at how predictions matched reality, while recall or sensitivity looks at reality matched the prediction. Our model's **precision** score is **85%** for default loans and **100%** for healthy loans, and the model's **recall** score is **91%** for default loans and **99%** for healthy loans.
  * The **F1 score** is a weighted average of the precision and recall scores. Our model's F1 score is **88%**.
* **Machine Learning Model 2:**

  * Our **balanced accuracy score** and our **accuracy** score are both **99%**. The balanced accuracy score provides a measure of the performance of our model when the dataset is imbalanced. In our dataset however, we have an equal number in each class, 56271. Hence the balanced accuracy score is the same as the accuracy score.
  * Based on the **confusion matrix**, the model accurately accepted 18649 healthy loans and rejected 615 high-risk loans. However, the model also incorrectly rejected 116 healthy loans and incorrectly accepted 4 high-risk loans.
  * Our model's **precision** score is **84%** for default loans and **100%** for healthy loans. The model's **recall** score is **99%** for default loans and **99%** for healthy loans.
  * Our model's **F1 score** (the weighted average of precision and recall scores) is **91%**.

## Summary

Both of the models have acceptable fit to the data, with a balanced accuracy of 95% in model 1 and an accuracy of 99% in model 2. Model appears to perform better than model 1, as the accuracy of model 2 is better than the balanced accuracy of model 1. Note: We are using balanced accuracy for model 1 because the distribution of the data between the classes (healthy vs. default) was not balanced.

In our model, we are trying to maximize the number of low-risk loans that are identified as healthy, and we want to reduce the number of loans given out that are high-risk. Model 1 accepted 56 high-risk loans, but model 2 only accepted 4 high-risk loans. 

The F1 score, which accounts for the precision and recall of the models, was better for model 2 than model. 

Based on this, **model 2** appears to perform better than model 1.
