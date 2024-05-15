# Module 20: Credit Risk Classification
All work is present in the "credit_risk_classification" Jupyter notebook. The expanded analysis is below

## Overview
The purpose of this analysis is to determine how well a logistic regression model performs on the problem of predicting whether a loan is healthy or high-risk based on a number of other loan features. By generating a LR model and running a split dataset through it, we can see how well it recognizes these loan classes in test data.
- Accuracy: This represents the model's overall correctness. While the 99% accuracy of our model seems impresssive at first, the class imbalance in the dataset means we should be more doubtful about its performance.
- Precision: This represents how many of the target class are correctly identified as such. This is the major stumbling block in the model's performance. High-risk loan precision is the lowest score in the classification report, meaning that the model misses about 15% of all high-risk loans present in the test dataset.
- Recall: This represents how many of the model's predictions of the target class are actually the target. Recall is higher across classes, though we still see reduced performance for high-risk loans. This means we are incorrectly labeling some healthy loans as high-risk instead.
Given that the company is likely more concerned about the correct and complete identification of high-risk loans, I would be hesitant to recommend this model. It's performance is significantly lower for those loans due to the large class imbalance in the overall dataset.
