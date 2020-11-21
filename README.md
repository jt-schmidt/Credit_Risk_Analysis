# Credit_Risk_Analysis
UT Data Analytics &amp; Visualization Bootcamp:  Module 17 -- Machine Learning using Python

## Overview
For Module 17 Challenge, Machine Learning Models are evaluated against financial data to determine credit risk.  This is performed within Python & Jupyter Notebook in Anaconda.  
Key resources utilized are:
* [sklearn](https://scikit-learn.org/stable/)
* [imbalanced learn](https://pypi.org/project/imbalanced-learn/)

Comments on raw data provided:
* 2019 Q1 Financial Data
* 115,676 rows by 144 columns

Goal is to compare 6 Machine Learning Models against the raw data set & provide judgement on the models based on observations for Accuracy, Precision, Recall:
* Naive Random Oversampling
* SMOTE Oversampling
* Undersampling
* Combination (Over and Under) Sampling
* Balanced Random Forest Classifier
* Easy Ensemble AdaBoost Classifier

## Results
<!-- There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models -->

|  #  | Machine Learning Model | Balanced Accuracy | Precision* | Recall* | Observations |
| --- | ---------------------- | ----------------- | --------- | ------------------ | -------- |
| 1 | Naive Random Oversampling | 0.6480 | 0.99 | 0.60 | N/A |
| 2 | SMOTE Oversampling | 0.6625 | 0.99 | 0.69 | N/A |
| 3 | Undersampling | 0.6625 | 0.99 | 0.42 | Lowest Sensitivity |
| 4 | Combination (Over and Under) Sampling | 0.5443 | 0.99 | 0.58 | Lowest Accuracy |
| 5 | Balanced Random Forest Classifier | 0.6830 | 1.00 | 1.00 | N/A |
| 6 | Easy Ensemble AdaBoost Classifier | 0.7325 | 1.00 | 1.00 | Highest Accuracy / Highest Sensivity |

*NOTE: 
* Precision is essentially equivalent among all models (0.99 ~ 1.00)
* Recall = Sensitivity
 
Reference:  [Judging Machine Learning Models](https://www.jeremyjordan.me/evaluating-a-machine-learning-model/#:~:text=The%20three%20main%20metrics%20used,the%20number%20of%20total%20predictions.)

## Summary
<!--There is a recommendation on which model to use, or there is no recommendation with a justification-->

Best overall model to use is "Easy Ensemble AdaBoost Classifier" based on higher Balanced Accuracy & Sensitivity result.  
Precision had no factor in decision since all models were essentially equivalent.  

[F-score](https://en.wikipedia.org/wiki/F-score) should also be considered when evaluating the models.  
Although not requested as focus as part of the challenge, review of F-Score finds:
* Naive Random Oversampling = 0.75
* SMOTE Oversampling = 0.81 
* Undersampling = 0.58
* Combination (Over and Under) Sampling = 0.72
* Balanced Random Forest Classifier = 1.00
* Easy Ensemble AdaBoost Classifier = 1.00

Of interest here is that Random Forest & Adaboost both have same F-Score (1.00), but Balanced Accuracy is less for Random Forest vs AdaBoost (0.6830 < 0.7325).  
This reinforces a need to look at overall results in detail versus determination through single score selection.
