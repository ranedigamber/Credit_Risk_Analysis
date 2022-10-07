# Credit_Risk_Analysis
# Overview of the Project
There exit an inherent unbalanced classification problem with Credit Risk as the good loans typicaly outnumber the risky loans.In this challenge we have used different techniques to train and evaluate models with unbalanced classes. We have specifically used imbalance-learn and scikit-learn libraries to build and evaluate models using resampling.
On the provided dataset we have used RandomOverSampler and SMOTE algorithms to oversample the data. ClusterCentroids algorithm to undersample the dataset and use a combinitorial approach of under- and oversampling using the SMOTEEN alogrithm. 
We compared two new machine learning models that reduce bias BalancedRandomForestClassifier and EasyEnsembleClassifier to predict credit risk.

## Results
The results of these machine learning models can be evaluated by output parameters such as precision, recall, and balanced accuracy

### Native Random Oversampling
The image is the output analysis for this model. 
Balanced accuracy = ~0.63
From this analysis it can be concurred that the precision for high-risk loans is low and that for low-risk loans is high.
Also, the recall for both these types of loans is similar

![Native Random Oversampling](https://user-images.githubusercontent.com/107159218/194452470-3bdc84ec-bb71-4df7-9c64-ba7d5c13c937.PNG)

### SMOTE Oversampling
The image is the output analysis for this model
Balanced accuracy = ~0.63
The precision for low and high-risk loan is similar to the previous model.

![SMOTE Oversampling](https://user-images.githubusercontent.com/107159218/194452982-4d734fc0-0e98-40ad-b7a0-cf18ff4d2c0d.PNG)

### Undersampling
The image is the output analysis for this model
Balanced accuracy = ~0.63
Similar to the above two models the precision for high-risk loans is low and that for low-risk loans is high.
However the recall for these two loan type is different. 

![Undersampling](https://user-images.githubusercontent.com/107159218/194453327-001d6015-1e48-4f94-8f79-cbfa16f04e60.PNG)

### Combination Under-Over Sampling
The image below is the output analysis for this model
Balanced accuracy = ~0.51
The precision for low-risk and high-risk loan remains the same as the above three models.
The recall for these two loan types is different. That for high-risk is 0.78 and that for low-risk is 0.58

![Combination_Under-Over Sampling](https://user-images.githubusercontent.com/107159218/194453637-b89b7204-9729-4c16-a35f-f67264c49260.PNG)

### Balanced Random Forest Classifier
The image below is the output analysis for this model
Balanced accuracy = ~0.79
The precision for low-risk and high-risk is similar to other models disscused so far. 
However the recall for both the loan types is substantially different. With that for high-risk = 0.91 and that for the low-risk = 0.67

![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/107159218/194454166-d2f93df6-b651-4524-9fbf-fb574c097924.PNG)

### Easy Ensemble AdaBoost Classifier
The image below is the output analysis for this model
Balance accuracy = ~0.93
The precision for the low-risk and high-risk loans are along the same trend lines as the ones above. 
The recall for both these loan types is similar.

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/107159218/194455406-7bd89270-3e12-4785-9515-f22f72c41947.PNG)

## Summary Result
Easy Ensemble AdaBoost Classifer with balanced accuracy and recall (for both loans) is much close to 1 that all the other models used for machine learning. It should be noted that ideally the closer these scores are to 1 the better the machine learning model. 

