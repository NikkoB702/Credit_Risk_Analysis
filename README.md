# Credit_Risk_Analysis

## Overview:

LendingClub, a peer-to-peer lending service has asked us to use their available dataset and predict credit risk using machine learning techniques. We will need to use imbalanced-learn and scikit-learn libraries due to the unbalanced classes. When it comes to risk management for loans, we will look for more of a precision-based model to determine our success rates. By utilizing various algorithms and coupling them with some machine learning models we will determine which is a better fit. 

## Results

##### SMOTE Oversampling

![Smote_Oversampling](https://user-images.githubusercontent.com/80132877/212374049-38dd578a-34ed-43c1-a536-7b7955065a75.png)

##### Naive Random Oversampling

![Naive_Random_Oversampling](https://user-images.githubusercontent.com/80132877/212374173-f75b27bb-8836-47d5-97a3-012c93b806b2.png)

##### Undersampling

![Undersampling](https://user-images.githubusercontent.com/80132877/212374213-73523c3c-b3da-4f15-88c4-b2f387426641.png)

##### Combination Sampling

![Combo_OV_un](https://user-images.githubusercontent.com/80132877/212374266-b845070d-de6c-4139-b70f-25516f6c1708.png)

## Models

##### Balanced Random Forest Classifier

![Balanced_Random_Forest_Classifier](https://user-images.githubusercontent.com/80132877/212374359-3c491f0e-ca0e-4395-90f5-1a584264b993.png)

##### Easy Ensemble AdaBoost Classifier

![Easy_Ensemble_AdaBoost_Classifier](https://user-images.githubusercontent.com/80132877/212374428-d9b3a9a9-2386-4490-9d13-3f98b031f106.png)


## Summary

Briefly it appears that the Easy Ensemble classifier outperforms the other models. The accuracy rate is a touch over 93%. The Easy Ensemble classifier also outperforms the other models in categories like precision, recall and F1 score. However, based on further analysis we see a wide difference between precision and recall and unfortunately it goes against what we desire. Our recall rate is at 94% while the precision rate is a mere 9%. This means that we have an aggressive model which might result in several false positives. Conversely, our F1 score runs at 16% which indicates a pronounced imbalance between sensitivity and precision. I would recommend a model that is both accurate and strikes a balance between precision and recall.
