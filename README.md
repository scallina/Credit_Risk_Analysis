# Credit_Risk_Analysis

## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. In this project, I employed different techniques to train and evaluate machine learning models with unbalanced classes in order to find the model that best predict risky vs safer loan applications. My credit card credit dataset was pulled from LendingClub, a peer-to-peer lending services company.  

First, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. I also used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 
Next, I used the BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

In the summary section, I rated the performance of these models and make a written recommendation on whether they should be used to predict credit risk.


## Results
- Random Oversampling (accuracy .59)
![image](https://github.com/scallina/Credit_Risk_Analysis/blob/main/Images/Random%20Oversampling.png)

- SMOTE Undersampling (accuracy .65)
![image](https://github.com/scallina/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Oversampling.png)

- Undersampling (accuracy .65)
![image](https://github.com/scallina/Credit_Risk_Analysis/blob/main/Images/Undersampling.png)

- Combination Sampling (accuracy .54)
![image](https://github.com/scallina/Credit_Risk_Analysis/blob/main/Images/Combination%20Sampling.png)

- Random Forest Sampling (accuracy .66)
![image](https://github.com/scallina/Credit_Risk_Analysis/blob/main/Images/Random%20Forest.png)

- EasyEnsemble (accuracy .66)
![image](https://github.com/scallina/Credit_Risk_Analysis/blob/main/Images/Ensemble%20Adaboost.png)

## Summary 

According to these results, the Random Forest model performed the best in precision when it comes to identifying low-risk loan applications, which is more fitting for this study. In addition, the model using Random Forest also had the highest sensitivity among the 6, which would make it the strongest model for reliably predicting low-risk loan applicants in other datasets.  
