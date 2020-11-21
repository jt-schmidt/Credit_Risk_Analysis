# Credit_Risk_Analysis
UT Data Analytics &amp; Visualization Bootcamp:  Module 17 -- Machine Learning using Python

## Overview

## Results
<!-- There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models -->


|  #  | Machine Learning Model | Balanced Accuracy | Precision | Recall/Sensitivity | Observations |
| --- | ---------------------- | ----------------- | --------- | ------------------ | -------- |
| 1 | Naive Random Oversampling | 0.6480 | 0.99 | 0.60 | N/A |
| 2 | SMOTE Oversampling | 0.6625 | 0.99 | 0.69 | N/A |
| 3 | Undersampling | 0.6625 | 0.99 | 0.42 | Lowest Sensitivity |
| 4 | Combination (Over and Under) Sampling | 0.5443 | 0.99 | 0.58 | Lowest Accuracy |
| 5 | Balanced Random Forest Classifier | 0.6830 | 1.00 | 1.00 | N/A |
| 6 | Easy Ensemble AdaBoost Classifier | 0.7325 | 1.00 | 1.00 | Highest Accuracy / Highest Precision / Highest Sensivity |

NOTE: Precision is essentially equivalent among all models (0.99 ~ 1.00)
 
Reference:  [Judging Machine Learning Models](https://www.jeremyjordan.me/evaluating-a-machine-learning-model/#:~:text=The%20three%20main%20metrics%20used,the%20number%20of%20total%20predictions.)




## Summary
<!--There is a recommendation on which model to use, or there is no recommendation with a justification-->
