# Credit_risk_analysis
In Credit Risk Analysis, we have to apply machine learning  to predict credit risk. Resampling, SMOTEENN and Emsemble classifiers methods  were used.
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. 

In this project, we used Python to build and evaluate several machine learning models to predict credit risk:

  * oversample the data using the RandomOverSampler and SMOTE algorithms.
  * Undersample the data using the ClusterCentroids algorithm.
  * a combinatorial approach of oversampling and undersampling using the SMOTEENN algorithm.
  * compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.
  * evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.


We used imbalance-learn and scikit-learn libraries to build and evaluate models using resampling.



![png_Ch17p1](https://github.com/Ruma-T/Credit_risk_analysis/blob/main/Ch17p1.PNG)












### Naive Random Oversampling

The balanced accuracy score is 65.12%.

![png_Ch17p4](https://github.com/Ruma-T/Credit_risk_analysis/blob/main/Ch17p4.PNG)







### SMOTE Oversampling

The balanced accuracy score is 51.79%.
![png_Ch17p5](https://github.com/Ruma-T/Credit_risk_analysis/blob/main/Ch17p5.PNG)





### Undersampling
The balanced accuracy score is 62.67%.
![png_Ch17p6](https://github.com/Ruma-T/Credit_risk_analysis/blob/main/Ch17p6.PNG)





### Balanced Random Forest Classifier
The balanced accuracy score is 62.67%.

![png_Ch17p2](https://github.com/Ruma-T/Credit_risk_analysis/blob/main/Ch17p2.PNG)


The balanced accuracy score is 62.67%.
![png_Ch17p3](https://github.com/Ruma-T/Credit_risk_analysis/blob/main/Ch17p3.PNG)

### Summary  3
All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high.
The Ensemble models brought a lot more improvment specially on the sensitivity of the high risk credits.
The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit. On another hand, with a low precision, a lot of low risk credits are still falsely detected as high risk which would penalize the bank's credit strategy and infer on its revenue by missing those business opportunities.
For those reasons I would not recommend the bank to use any of these models to predict credit risk.
