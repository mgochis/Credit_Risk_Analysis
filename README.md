# Credit_Risk_Analysis
 
## Overview

In this project, we used machine learning to predict credit risk for a peer-to-peer lending service. Credit risk is an inherently unbalanced classification problem since most loans are not considered risky. I used a variety of different techniques to train and evaluate the peer-to-peer lending data.

## Results

- Naive Random Oversampling
    - When reviewing the imbalanced classification report we see that the precision score for low-risk loans is 1.00 meaning there is a near perfect prediction on low risk loans. High risk loan precision score was only 0.01 which means this model is not great at predicting if a loan is high risk. This method is good at predicting low risk loans, but not at predicting high risk.
    ![Naive Random Oversampling Image](https://github.com/mgochis/Credit_Risk_Analysis/blob/32e7b5987f30cf590a17528360da9be91c356b15/images/Naive%20Random%20Oversampling.png)
- SMOTE Oversampling
    - There is little difference from the results between the previous model and this model. Both models are not great for predicting if a loan is high risk or low risk. 
    ![SMOTE Oversampling Image](https://github.com/mgochis/Credit_Risk_Analysis/blob/32e7b5987f30cf590a17528360da9be91c356b15/images/SMOTE%20Oversampling.png)
- Under sampling
    - Under sampling performed slightly better when predicting high risk loans when compared to the previous two models. The accuracy score is rather low at 67% so under sampling may not be the best model for predicting risk for a loan. 
    ![Under sampling](https://github.com/mgochis/Credit_Risk_Analysis/blob/32e7b5987f30cf590a17528360da9be91c356b15/images/Undersampling.png)
- Combination (Over and Under) Sampling
    - This method oversamples the minority class and under samples the majority class. The results have a low accuracy score, low precision scores and low recall scores. This is not a good method to use when trying to predict credit risk
    ![Combination (Over and Under) Sampling](https://github.com/mgochis/Credit_Risk_Analysis/blob/32e7b5987f30cf590a17528360da9be91c356b15/images/Combination%20(Over%20and%20Under)%20Sampling.png)
- Balanced Random Forest Classifier
    - This method is slightly better than the previous methods with an accuracy score of 79%. So far, this is best method for predicting loan risk. 
    ![Balanced Random Forest Classifier](https://github.com/mgochis/Credit_Risk_Analysis/blob/32e7b5987f30cf590a17528360da9be91c356b15/images/Balanced%20Random%20Forest%20Classifier.png)
- Easy Ensemble AdaBoost Classifier
    - This model is by far the best for predicting high risk and low risk loans. The accuracy score of 93% gives way more confidence than previous methods used. This is the recommended model to predict loan riskiness. 
    ![Easy Ensemble AdaBoost Classifier](https://github.com/mgochis/Credit_Risk_Analysis/blob/32e7b5987f30cf590a17528360da9be91c356b15/images/Easy%20Ensemble%20AdaBoost%20Classifier.png)

## Summary

We used six different models to try to predict how risky a loan is using data from a peer-to-peer lending service. Of the six tested, by far the best model is the Easy Ensemble AdaBoost Classifier and should be used to predict loan riskiness. The accuracy score of 93% and all other scores over 90% this is a reliable model to use. 

