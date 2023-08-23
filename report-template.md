# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of the analysis is to train and evaluate a model on loan risk. The dataset used for the project is historical lending activity from a peer-to-peer lending services company. Loans are identified as either defaulting (1) or healthy (0).

The model will identify the creditworthiness of borrowers as either high-risk (unhealthy loan/defaulting) or low-risk (healthy loan).

To complete this project, I created two models. The first model is the training model. For this model a portion of the data was used to 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:

  * Our **balanced accuracy score** is **95%**. The balanced accuracy score takes into account the sensitivity (true positive rate) and the specificity (true negative rate). The balanced accuracy score is measures the performance of our model, especially with imbalanced datasets. In our dataset, we have 75036 loans that were rejected, but only 2500 that were accepted. Since our data is imbalanced, the balanced accuracy score serves are our metric for the performance of our model.
  * Based on the **confusion matrix**, the model accurately accepted 563 healthy loans and rejected 18663 high-risk loans. However, the model also incorrectly rejected 56 healthy loans and incorrectly accepted 102 high-risk loans.
  * The model's **accuracy score** is **99%**, which means that the model correctly predicted 99% of all loans in the dataset.
  * **Precision** measures on how many of the positive predictions in the model were actually positive (or the proportion of positive predictions that were actually correct). Our model's precision score is **85%**.
  * The **recall or sensitivity** score measures how many of the actual positive instances were correctly predicted as positive (or the proportion of actual positives that were identified correctly). The model's recall score is **91%**.
  * The **F1 score** is a weighted average of the precision and recall scores. Our model's F1 score is **88%**.
* Machine Learning Model 2:

  * Our **balanced accuracy score** is **99%**. The balanced accuracy score takes into account the sensitivity (true positive rate) and the specificity (true negative rate). The balanced accuracy score is measures the performance of our model, especially with imbalanced datasets. In our dataset, we have an equal number in each class, 56271.
  * Based on the **confusion matrix**, the model accurately accepted 615 healthy loans and rejected 18649 high-risk loans. However, the model also incorrectly rejected 4 healthy loans and incorrectly accepted 116 high-risk loans.
  * The model's **accuracy score** is **99%**, which means that the model correctly predicted 99% of all loans in the dataset.
  * **Precision** measures on how many of the positive predictions in the model were actually positive (or the proportion of positive predictions that were actually correct). Our model's precision score is **84%**.
  * The **recall or sensitivity** score measures how many of the actual positive instances were correctly predicted as positive (or the proportion of actual positives that were identified correctly). The model's recall score is **99%**.
  * The **F1 score** is a weighted average of the precision and recall scores. Our model's F1 score is **91%**.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
