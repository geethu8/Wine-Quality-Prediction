# Wine-Quality-Prediction

## Supervised Learning Classification


### Project Objective:
To develop a predictive model that helps us identify the quality of the wine. The red variants of Portuguese Vinho Verde wine are used. Their compositions including various chemicals which determine the quality of the wine are the predictors of this classification problem. The classes are ordered and not balanced (e.g. there are much more normal wines than excellent or poor ones).


### Data:
The data used in this project is a dataset containing features related to the composition of the wine. The dataset has 1143 observations and 13 variables. The data has all numerical variables and has a high amount of outliers.


### Methods:
• Outlier Treatment: High amount of outliers were identified which were treated using the capping technique.

• Binning: It is the process of transforming numerical variables into their categorical counterparts. Since the occurrence of certain classes is very low the wine with a score less than or equal to 4 was classified as bad, the ones with a score above 7 is good and the rest are average. These were again encoded as 0,1 and 2 for model prediction.

• SMOTE Technique: SMOTE (Synthetic Minority Over-sampling Technique) is a technique used to balance imbalanced data. It generates synthetic samples of the minority class to increase its representation in the dataset. This was because after feature engineering the number of average classes was very high compared to good and bad.

• Standard Scaler: It is used to resize the distribution of values so that the mean of the observed values is 0 and the standard deviation is 1. It brings all the variables to the same scale. 

• Yeo Johnson Transformation:  Used to create normally distributed variables from non-normal ones. From the histograms it is to be seen that data is skewed thus we bring it to normal form for better performance using transformation. Yeo-Johnson can work with negative values also.

• Model Building: Decision Tree with and without hyperparameter tuning, KNN, Random Forest with and without hyperparameter tuning, Bagging Classifier, and XGBoost Classifier are the main models used to solve this problem statement. 

### Conclusion:
Accuracy is the main metric used in this case. Meanwhile, the f1score for each class will be considered in order to analyze which classification model can identify all the classes appropriately so that it can be used for future predictions of the wine quality as well. 
