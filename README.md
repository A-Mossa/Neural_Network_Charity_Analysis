# Neural_Network_Charity_Analysis

## Overview of the project

Utilizing Neural Network Machine Learning model to facilitate the prediction of new applicantions, and determine the potential success when Alphabet Soup funding is granted. 
The dataset used contatined information about application type, classification, field, status, current income, and if the specific application was successful or not.

## Results

### Data Preprocessing
![Ovrsmpl Acc](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/Ovrsmpl%20Accuracy.png)
- Balanced Accuracy Score of 64%

![Ovrsmpl CM](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/Ovrsmpl%20CM.png)
- High Risk Precision of 1% and Sensitivity of 61%
- Low Risk Precision of 100% and Sensitivity of 68%
- F1 value of 2% for High Risk

![Ovrsmpl Clr](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/Ovrsmpl%20Clr.png)

### Oversampling  with SMOTE

![SMOTE Smt](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/SMOTE%20acc.png)
- Balanced Accuracy Score of 65.2%

![SMOTE CM](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/SMOTE%20CM.png)
- High Risk Precision of 1% and Sensitivity of 67%
- Low Risk Precision of 100% and Sensitivity of 64%
- F1 value of 2% for High Risk

![SMOTE CM](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/SMOTE%20Clr.png)

### Undersampling with ClusterCentroids

![CC Acc](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/Undrsmpl%20Acc.png)
- Balanced Accuracy Score of 52%

![CC CM](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/Undrsmpl%20CM.png)
- High Risk Precision of 1% and Sensitivity of 57%
- Low Risk Precision of 100% and Sensitivity of 47%
- F1 value of 1% for High Risk

![CC Clr](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/Undrsmpl%20Clr.png)

### Combination Over and Undersampling with SMOTEENN

![Comp Acc](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/Comp%20Clr.png)
- Balanced Accuracy Score of 64%

![Comp CM](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/Comp%20CM.png)
- High Risk Precision of 1% and Sensitivity of 70%
- Low Risk Precision of 100% and Sensitivity of 58%
- F1 value of 2% for High Risk

![Comp Clr](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/Comp%20Clr.png)

### Ensemble learner with BalancedRandomForestClassifier

![blrf Acc](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/blrf%20Acc.png)
- Balanced Accuracy Score of 78.8%

![blrf Cm](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/blrf%20CM.png)
- High Risk Precision of 3% and Sensitivity of 70%
- Low Risk Precision of 100% and Sensitivity of 87%
- F1 value of 6% for High Risk which is a noticable jump from previous models

![blrf Clr](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/blrf%20Clr.png)

### Ensemble learner with EasyEnsembleClassifier

![ee Acc](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/EE%20Acc.png)
- Balanced Accuracy Score of 93.1% !

![ee Cm](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/EE%20CM.png)
- High Risk Precision of 9% and Sensitivity of 92%
- Low Risk Precision of 100% and Sensitivity of 94%
- F1 value of 16% for High Risk which is significantly higher than all other models !

![ee Clr](https://github.com/A-Mossa/Credit_Risk_Analysis/blob/main/Imgs/EE%20Clr.png)

## Summary

It is without a doubt that EasyEnsemble Classifier is the superior model for this use case because it yielded the best results out of all the six models trained.
its accuracy was an astonishing 93.1%, with 9% accuracy for high risk applications, and the highest sensitivity of 92%. Same can be said about this model's performance in detecting low risk loan applications with stats of 94% accuracy and an overall F1 score of 16%.

Jill and I would recommend moving forward using EasyEnsembleClassifier as the model of choice when dealing with Credit Risk, as it demonstrated the highest performance and yields out of all models trained, until a better model with better results is found.
