# Credit_Risk_Analysis

## Overview of Credit Risk Analysis

In this project, I have been tasked with creating multiple iterations of supervised machine learning models to predict the risk level of issued loans based on a loan statistics dataset. The dataset contains 85 different independent variables, or features, that are input into six machine learning models to predict the loan status, namely, high-risk or low-risk. The dataset contains 68817 distinct loans, of which 80% are randomly selected to train the model and 20% to test the model. The six machine learning algorithms used  in this analysis are as follows:

- Logistic Regression with RandomOverSampler
- Logistic Regression with SMOTE
- Logistic Regression with ClusterCentroids
- Logistic Regression with SMOTEENN
- Balanced Random Forest Classifier
- Easy Ensemble AdaBoost Classifier

The above machine learning models were developed in python using Jupyter Notebook and importing the sklearn, imblearn, numpy and pandas python libraries. Various performance metrics were used to evaluate the accuracy, precision, and sensitivity of each model using a confusion matrix and classification report. The full set of resources and analysis results are shown below.

## Resources

- Data Sources: LoanStats_2019Q1.csv
- Software: Python 3.7, Jupyter Notebook, and sklearn and imblearn libraries

## Analysis Results

The set of performance results were derived using the following supervised machine learning models

- Logistic Regression with RandomOverSampler

<img width="710" alt="RandomOverSampler" src="https://user-images.githubusercontent.com/95327115/163744363-41939846-50ea-463c-b670-3dfe19bef33d.png">

This model has an accuracy of 63%, a precision of 1%, and a sensitivity of 63%.

- Logistic Regression with SMOTE

<img width="704" alt="SMOTE" src="https://user-images.githubusercontent.com/95327115/163744384-e6aa3dae-e7f1-4569-a2f0-a85d1f5980d0.png">


This model has an accuracy of 65%, a precision of 1%, and a sensitivity of 61%.

- Logistic Regression with ClusterCentroids

<img width="709" alt="ClusterCentroids" src="https://user-images.githubusercontent.com/95327115/163744399-eb1c6a60-323b-415f-9528-b776afc6f6a6.png">


This model has an accuracy of 50%, a precision of 1%, and a sensitivity of 56%.

- Logistic Regression with SMOTEENN

<img width="707" alt="SMOTEENN" src="https://user-images.githubusercontent.com/95327115/163744411-51c64b1d-9a81-4c0f-bbaf-0490d4efb6f9.png">


This model has an accuracy of 61%, a precision of 1%, and a sensitivity of 67%.

- Balanced Random Forest Classifier

<img width="453" alt="RandomForestClassifier" src="https://user-images.githubusercontent.com/95327115/163744421-21796eea-e108-412c-add5-77bf4c541815.png">


This model has an accuracy of 91%, a precision of 4%, and a sensitivity of 68%.

- Easy Ensemble AdaBoost Classifier

<img width="455" alt="EasyEnsembleClassifier" src="https://user-images.githubusercontent.com/95327115/163744433-bf21db1f-2a1f-44d9-bc22-050f2782c231.png">

This model has an accuracy of 94%, a precision of 7%, and a sensitivity of 91%.

## Summary Statistics on Suspension Coils

Based on the performance results of the models, the Easy Emsemble AdaBoost Classifier has the highest balanced accuracy, precision, and sensitivity. I would recommend using the Easy Emsemble AdaBoost Classifier model to predict the credit risk on the provided feature criteria. This model has the greatest accuracy and will correctly determine if the loan is high risk 91% of the time. Since we are more likely to value sensitivity over precision, this is the best model to use to capture as many high risk loans are possible for further evaluation. The Random Forest Classifier and SMOTEENN models are also worthwhile candidates, but will not provide results with nearly the same amount of confidence.
