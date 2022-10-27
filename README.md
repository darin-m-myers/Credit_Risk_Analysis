# Credit_Risk_Analysis
Credit_Risk_Analysis using Machine Learning and Python

## Overview
The purpose of this analysis is to perform a comparison of various machine learning resampling techniques to determine the best model for predicting credit risk.

## Results
- Naive Random Oversampling
  The Accuracy Score was 62.9% which was the second lowest of all methods.
  The Precision was 0.01 for high_risk and 1.00 for low_risk. Not a great method for determining high risk.
  The Recall was 0.63 for high_risk and 0.62 for low risk. Ok, but not great for collecting all high_risk instances.
  
- SMOTE Oversampling
  The Accuracy Score was 66.3% which was the highest of all the Oversampling and Understampling methods, but third out of all methods.
  The Precision was 0.01 for high_risk and 1.00 for low_risk. Not a great method for determining high risk.
  The Recall was 0.63 for high_risk and 0.69 for low risk. Ok, but not great for collecting all high_risk instances.
  
- Undersampling
  The Accuracy Score was 57.5% which was by far the second worst of all methods.
  The Precision was 0.01 for high_risk and 1.00 for low_risk. Not a great method for determining high risk.
  The Recall was 0.62 for high_risk and 0.53 for low risk. Ok, but not great for collecting all high_risk instances.
  
- Combination (SMOTEENN)
  The Accuracy Score was 64.8% which was the third lowest of all methods.
  The Precision was 0.01 for high_risk and 1.00 for low_risk. Not a great method for determining high risk.
  The Recall was 0.72 for high_risk and 0.57 for low risk. An improvement to collecting all high risk instances over the previous methods.

- Balanced Random Forest Classifier
  The Accuracy Score was 76.5% which was the second hightes of all methods.
  The Precision was 0.03 for high_risk and 1.00 for low_risk. Not a great method for determining high risk.
  The Recall was 0.65 for high_risk and 0.88 for low risk. Ok, but not great for collecting all high_risk instances.

- Easy Ensemble AdaBoost Classifier
  The Accuracy Score was 93.2% which was the second hightes of all methods.
  The Precision was 0.09 for high_risk and 1.00 for low_risk. Not a great method for determining high risk.
  The Recall was 0.92 for high_risk and 0.94 for low risk. Much higher confidence for collecting all high_risk instances.


Figure 1.1 - Credit Risk Resampling Techniques

![image](https://user-images.githubusercontent.com/107961905/198178829-262b95ad-06c6-4cea-abca-4f088bf93504.png)

Figure 1.2 - Classification Reports of Oversampling and Undersampling Techniques

![image](https://user-images.githubusercontent.com/107961905/198178725-489f3f50-e30a-42f4-8d4f-a2c66241380c.png)

Figure 1.3 - Credit Risk Classification Reports of Ensemble Classification Techinques

![image](https://user-images.githubusercontent.com/107961905/198178734-510038f4-f71d-4143-86af-384adc698ce2.png)

## Summary
### Summary of Results
Overall the Easy Ensemble AdaBoost Classifier the very best method and Undersampling produced the worst results. The precision on for high_risk was incredibly low for all methods, so the current data was not really sufficient for accurately identifiying only the high_risk instances.

### Recommendation
If I had to pick a model, the Easy Ensemble AdaBoost Classifier would be the one to go with. Overall, I would not recommend any of these models with the current dataset as the precision is very low. It would be very difficult to actually determine whether a particular instance was an actual credit risk from the amount of data that we have. The Recall was ok for the AdaBoost, but we really need more of the high_risk data to train the model on before we can get a more accurate result. 