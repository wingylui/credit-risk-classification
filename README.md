# Module 20 Challenge: Supervised Learning
---

<b>Programming language:</b> Python <br />
<b>Package used:</b>sklearn, pandas and numpy <br />
<b>Main script:</b> [credit_risk_classification.ipynb](https://github.com/wingylui/credit-risk-classification/blob/main/credit_risk_classification.ipynb)<br />
<b>Dataset:</b> [lending_data.csv](https://github.com/wingylui/credit-risk-classification/blob/main/Resources/lending_data.csv)

---
## Overview of the Analysis

In this challenge, a model was builded to identify the creditworthiness of borrowers by using a dataset with historical lending activity from a peer-to-peer lending services company. The dataset consist of the detail information of both healthy loan (n = 75,036) and high-risk loan (n = 2,500), including borrower income, interest rate, loan size etc.</br>

To train a model to predict the creditworthiness of borrowers, the dataset was firstly split into texting and training dataset using `train_test_split`; and then, a Logistic Regression model was created by using `LogisticRegression`. As there is a big sample size difference between healthy and high-risk loan, we also tried to create a model with resampled training dataset (using `RandomOverSampler`) and compared its performance to the performance of model trained with original training data.

---
## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model trained by orignial data:
  * Accuracy : 0.9520
  * Precision : 1.00 for healthy loan and 0.85 for high-risk loan
  * Recall scores : 0.99 for healthy loan and 0.91 for high-risk loan</br>

* Machine Learning Model trained after resampled by ramdom over sampler:
  * Accuracy : 0.9515
  * Precision : 0.92 for healthy loan and 0.99 for high-risk loan
  * Recall scores : 1.00 for healthy loan and 0.91 for high-risk loan

---

## Summary

To conclude, based on the above results, both models perform with high accuracy on predicting healthy loan while the model trained with resampled data predicts high-risk loan better. Since predicting high-risk loan is much more important for credit risk evaluation, I will recommend the model trained with resampled data.


---
<b>Score for this assessment:</b> has not been graded yet <br />
<b>References:</b><br />
Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.

