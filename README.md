# Credit_Risk_Analysis

## Overview
For this project, I used supervised machine learning to predict credit risk. Using Python and the Scikit-learn library, I built and evaluated several models using different algorithms. The goal is to help lending institutions find the right balance of choosing the good credit risks so they can earn revenue by collecting interest while minimizing the risk that borrowers will default on their loans which causes lenders to lose money. 

## Results

The first machine learning models that I used were RandomOverSampler and SMOTE algorithms which oversample data. Next, I undersampled the data using the ClusterCentroids model. I then used combinatorial approach of over- and undersampling using the SMOTEENN model. Finally, I used two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.



•	Accuracy measures how successful the model was in predicting the testing set by comparing the difference between its predicted values and actual values. It is calculated as follows: 

    True Positives + True Negatives / (True Positives + True Negatives + False Positives + False Negatives)

-	Sample 1 – Naïve Random Oversampling: 0.64
-	Sample 2 – SMOTE Oversampling: 0.66
-	Sample 3 – Undersampling: 0.66
-	Sample 4 – Combination (Over and Under) Sampling: 0.54
-	Sample 5 – Balanced Random Forest Classifier: 0.79
-	Sample 6 – Easy Ensemble AdaBoost Classifier: 0.93

•	Precision measures the reliability of a positive classification. It is calculated as follows: 

    True Positives / (True Positives + False Positives)

-	Sample 1 – Naïve Random Oversampling: 0.99
-	Sample 2 – SMOTE Oversampling: 0.99
-	Sample 3 – Undersampling: 0.99
-	Sample 4 – Combination (Over and Under) Sampling: 0.99
-	Sample 5 – Balanced Random Forest Classifier: 0.99
-	Sample 6 – Easy Ensemble AdaBoost Classifier: 0.99

•	Sensitivity/Recall is a measure of how many observations with a positive condition will be correctly predicted. It is calculated as follows:

    True Positives / (True Positives + False Negatives) 

-	Sample 1 – Naïve Random Oversampling: 0.60
-	Sample 2 – SMOTE Oversampling: 0.69
-	Sample 3 – Undersampling: 0.40
-	Sample 4 – Combination (Over and Under) Sampling: 0.59
-	Sample 5 – Balanced Random Forest Classifier: 0.87 
-	Sample 6 – Easy Ensemble AdaBoost Classifier: 0.94

•	F1 Score balances precision and sensitivity and is calculated as follows: 
    
    2 * (Precision * Sensitivity) / Precision + Sensitivity)

-	Sample 1 – Naïve Random Oversampling: 0.74
-	Sample 2 – SMOTE Oversampling: 0.81
-	Sample 3 – Undersampling: 0.56
-	Sample 4 – Combination (Over and Under) Sampling: 0.74
-	Sample 5 – Balanced Random Forest Classifier: 0.93
-	Sample 6 – Easy Ensemble AdaBoost Classifier: 0.97


Easy Ensemble AdaBoost Classifier Results are shown below: 

![Sample6_confusion_matrix2](https://user-images.githubusercontent.com/90162669/150695042-d4c1af8a-768a-4b13-9539-13f2b5ce1fc9.png)


![Sample6_classification_rpt](https://user-images.githubusercontent.com/90162669/150695047-fb9fe576-90db-4f7e-9c1f-19fd76a464f8.png)


## Summary
The EasyEnsembleClassifier outperformed all of the other models. All scores indicate that this model/algorithm does a very good job of predicting high/low risk loans. I recommend this tool is used to evaluate future loan requests.  
