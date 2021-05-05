# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of this analysis was to use a logistic regression model to compare two versions of the same dataset. The first version was the original and for the second version we used an oversampling technique.
* Explain what financial information the data was on, and what you needed to predict.
The financial information we analyzed was a dataset of historical lending activity from a peer-to-peer lending services company. We needed to predict the creditworthiness of borrowers.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
We were trying to predict the 'loan_status' variable, which was either 0 which means a healthy loan, or 1 which means a loan at risk of defaulting. In the original dataset there were 75036 healthy loans, and 2500 at risk of defaulting.
* Describe the stages of the machine learning process you went through as part of this analysis.
First we read the data, then we split the data into training and testing sets. Next (only for the second part) we oversampled the data. Next we fit a logistic regression model, made predictions, and evaluated the model.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
For this challenge, we used LogisticRegression() and RandomOverSampler().

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of both machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
      * The accuaracy score was .95. 
      * For the high-risk loans, the precsion was .85 and the recall was .91.
      * For healthy loans, the precsion was 1.00 and the recall was 0.99.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
      * The accuaracy score was .99. 
      * For the high-risk loans, the precsion was .84 and the recall was .99.
      * For healthy loans, the precsion was 1.00 and the recall was 0.99.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
Machine Learning Model 2, where we used oversampling performed a little bit better, as the accuracy score was higher and the recall was higher (although precision was barely lower).
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Absolutely. For this exercise, predicting loans at risk of defaulting was the most important problem we were trying to solve. The second model did a better job of that because we used the oversampling technique to represent that data more.
