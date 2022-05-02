# Credit Risk Analysis
  Challenge 17

## Project Overview
Using Machine learning, I have used 6 different models to create predictions on credit risk. Using a dataset from LendingClub, Supervised Learning with  imbalanced-learn and scikit-learn libraries is utilized to find the best model for prediction. I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I used the combinatorial approach of over and undersampling using the SMOTEENN algorithm. Once that was complete, I compared two machine learning models that reduce bias: BalancedRandomForestClassifier and EasyEnsembleClassifier. Results for the 6 different models are explored below.

### Resources
            Data Sources: LoanStats_2019Q1.csv
            
            Software: Jupyter Notebook

## Results
* Naive Random Oversampling: The balanced accuracy test is 64%, high risk precision is 1% with a recall of 66% and low risk precision is 100% with a recall of 62%.

<img width="1090" alt="Naive_Random_Oversampling" src="https://user-images.githubusercontent.com/96352625/166185570-23c6ae2f-3276-4644-80b4-cf174e458035.png">

* SMOTE Oversampling: The balanced accuracy test is 65%, high risk precision is 1% with a recall of 61% and low risk precision is 100% with a recall of 69%.

<img width="1087" alt="SMOTE_Oversampling" src="https://user-images.githubusercontent.com/96352625/166185602-ff1f6900-652c-48f4-bf71-724252b9ecf8.png">

* Undersampling: The balanced accuracy test is 65%, high risk precision is 1% with a recall of 69% and low risk precision is 100% with a recall of 40%.

<img width="1086" alt="Undersampling" src="https://user-images.githubusercontent.com/96352625/166185625-60ac205d-8642-477c-8818-d61dff70ad9f.png">

* Combination Over and Undersampling: The balanced accuracy test is 54%, high risk precision is 1% with a recall of 69% and low risk precision is 100% with a recall of 40%.

<img width="1085" alt="Combination" src="https://user-images.githubusercontent.com/96352625/166185642-fcb8cb3b-3e3c-4058-b7e8-400d96d4e99f.png">

* Balanced Random Forest Classifier: The balanced accuracy test is 79%, high risk precision is 3% with a recall of 70% and low risk precision is 100% with a recall of 87%.

<img width="1087" alt="Balanced_Random_Forest_Classifier" src="https://user-images.githubusercontent.com/96352625/166185759-78e18b85-e22e-4cf1-8a4a-2bdde9fe797a.png">

* Easy Ensemble AdaBoost Classifier: The balanced accuracy test is 93%, high risk precision is 9% with a recall of 92% and low risk precision is 100% with a recall of 94%.

<img width="1087" alt="Easy_Ensemble_AdaBoost_Classifier" src="https://user-images.githubusercontent.com/96352625/166185862-e0599b3b-50c4-4072-b91b-e35166852714.png">


## Summary
The 6 models revealed varying levels of accuracy and precision. The combination model, SMOTE oversampling model, Naive Random Over Sampler, and the undersampling model all had accuracy rates below 66% and don't make for the most ideal models. Those 4 are not recommended for future modelng use. However, the Easy Ensemble AdaBoost Classifier is the standout for reccomendation for future use. For high risk candidates, the sensitivity rate is 92% with a 9% precision rate and for low risk candidates the sensitivity rate is at 94% with a precision rate of 100%. These sensitivity results were much higher than any of the other models and it has a balanced accuracy test of 93%, 15% higher than the next best model. The Easy Ensemble AdaBoost Classifier is the best model to use for the supervised learning exercise of predicting credit risk.
