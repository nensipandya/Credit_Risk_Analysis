# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis:
------------------------------------------------------------------------------------------------------------------------------------------------------------

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Various libraries and algorithms were used to build and evaluate models using resampling including:

  1.imbalanced-learn
  
  2. scikit-learn
  
  3. RandomOverSampler
  
  4. SMOTE algorithms
  
  5. ClusterCentroids algorithm
  
  6. SMOTEENN algorithm
  
  7. BalancedRandomForestClassifier (bias reduction model)
  
  8. EasyEnsembleClassifier (bias reduction model)
  
 
## Purpose
------------------------------------------------------------------------------------------------------------------------------------------------------------
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

  1. Explain how a machine learning algorithm is used in data analytics.
  
  2. Create training and test groups from a given data set.

  3. Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.

  4. Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.

  5. Compare the advantages and disadvantages of each supervised learning algorithm.

  6. Determine which supervised learning algorithm is best used for a given data set or scenario.

  7. Use ensemble and resampling techniques to improve model performance.
  
  
## Results
---------------------------------------------------------------------------------------------------------------------------------------------------------------------

The results of the balanced accuracy score and the precision and recall scores of all six machine learning models are as follows:

### Naive Random Oversampling

![image](https://user-images.githubusercontent.com/107137215/195115972-d83b2547-7c16-4af2-9046-00a7e5c92704.png)

  -> Balanced Accuracy: 0.6366972052004142
  
  -> Precision: The precision is low for High-risk  loans and high for Low-rik loans.
  
  -> Recall(sensitivity) : High/Low risk = 0.62/0.65

### SMOTE Oversampling

![image](https://user-images.githubusercontent.com/107137215/195116202-bb32f386-7388-4e9e-9f6c-07aec850a47a.png)


  -> Balanced Accuracy: 0.6302712208564487
  
  -> Precision: The precision is low for High-risk  loans and high for Low-rik loans.
  
  -> Recall(sensitivity) : High/Low risk = 0.62/0.64
  
  
### Undersampling

![image](https://user-images.githubusercontent.com/107137215/195116564-a1e13c41-c786-47b6-a901-0263ca9530d3.png)


  -> Balanced Accuracy: 0.6302712208564487
  
  -> Precision: The precision is low for High-risk  loans and high for Low-rik loans.
  
  -> Recall(sensitivity) : High/Low risk = 0.59/0.43


### Combination (Over and Under) Sampling


![image](https://user-images.githubusercontent.com/107137215/195117004-4cf6cc90-e94a-4f02-93b8-2ae50d5c1eac.png)

  -> Balanced Accuracy:0.5102725100821478
  
  -> Precision: The precision is low for High-risk  loans and high for Low-rik loans.
  
  -> Recall(sensitivity) : High/Low risk = 0.70/0.57

### Balanced Random Forest Classifier

![image](https://user-images.githubusercontent.com/107137215/195120656-a572b1ca-29a6-4a7e-9538-1d6b01b80df1.png)

  -> Balanced Accuracy: 0.7877672625306695
  
  -> Precision: The precision is low for High-risk  loans and high for Low-rik loans.
  
  -> Recall(sensitivity) : High/Low risk = 0.67/0.91
  
### Easy Ensemble AdaBoost Classifier

![image](https://user-images.githubusercontent.com/107137215/195121131-f98835d2-4f6d-41e6-8dae-eb48b43cb761.png)


  -> Balanced Accuracy: 0.925427358175101
  
  -> Precision: The precision is low for High-risk  loans and high for Low-rik loans.
  
  -> Recall(sensitivity) : High/Low risk = 0.91/0.94
  
 ## Summary
 ------------------------------------------------------------------------------------------------------------------------------------------------------------------
When working with balanced accuracy, the highest compared accuracy between 0 and 1 and is closest to 1 is the best machine learning model. For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy. The other models were below .80 balanced accuracy. The precision for all models were similar and within an appropriate range. The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model. The Easy Ensemble AdaBoost Classifier had the highest recall score, making it the final best machine learning model to choose for further credit card analysis.





