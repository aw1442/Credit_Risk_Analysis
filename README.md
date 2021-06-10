# Credit_Risk_Analysis

## Overview of the analysis

Jill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results

Here are the results from the six machine learning models:

Naive Random Oversampling:

- Balanced accuracy score: 0.6669003388246291
- Precision score: 
  - high_risk: 0.01
  - low_risk: 1.00
  - avg / total: 0.99
- Recall score:
  - high_risk: 0.67
  - low_risk: 0.67
  - avg / total: 0.67

![image](https://user-images.githubusercontent.com/76754655/121602674-88438500-c9fc-11eb-9e59-adf3928b77e6.png)

![image](https://user-images.githubusercontent.com/76754655/121602712-942f4700-c9fc-11eb-9da2-3d5996f2b35c.png)

![image](https://user-images.githubusercontent.com/76754655/121602738-9d201880-c9fc-11eb-9ecf-28f4c30c00d3.png)

SMOTE Oversampling:

- Balanced accuracy score: 0.6269111763781621
- Precision score: 
  - high_risk: 0.01
  - low_risk: 1.00
  - avg / total: 0.99
- Recall score:
  - high_risk: 0.57
  - low_risk: 0.68
  - avg / total: 0.68

![image](https://user-images.githubusercontent.com/76754655/121602791-ac06cb00-c9fc-11eb-8fb1-c6e4e7107d84.png)

![image](https://user-images.githubusercontent.com/76754655/121602825-b5903300-c9fc-11eb-8cea-1b7186ccb3da.png)

![image](https://user-images.githubusercontent.com/76754655/121602849-c0e35e80-c9fc-11eb-9bd3-8f026550473e.png)

ClusterCentroids Undersampling:

- Balanced accuracy score: 0.5259577536853726
- Precision score: 
  - high_risk: 0.01
  - low_risk: 1.00
  - avg / total: 0.99
- Recall score:
  - high_risk: 0.59
  - low_risk: 0.47
  - avg / total: 0.47

![image](https://user-images.githubusercontent.com/76754655/121602933-e2dce100-c9fc-11eb-9638-e6103da1c040.png)

![image](https://user-images.githubusercontent.com/76754655/121602960-eb351c00-c9fc-11eb-97dc-19a2d67b1faa.png)

![image](https://user-images.githubusercontent.com/76754655/121602983-f38d5700-c9fc-11eb-9d46-849357e65e96.png)

SMOTEENN Combination (Over and Under) Sampling:

- Balanced accuracy score: 0.6066421310900806
- Precision score: 
  - high_risk: 0.01
  - low_risk: 1.00
  - avg / total: 0.99
- Recall score:
  - high_risk: 0.67
  - low_risk: 0.55
  - avg / total: 0.55

![image](https://user-images.githubusercontent.com/76754655/121603080-161f7000-c9fd-11eb-8529-1cf4575a0d3e.png)

![image](https://user-images.githubusercontent.com/76754655/121603100-1f104180-c9fd-11eb-88c5-100b581bac6a.png)

![image](https://user-images.githubusercontent.com/76754655/121603123-27687c80-c9fd-11eb-803d-5527d0590c6a.png)

Balanced Random Forest Classifier:

- Balanced accuracy score: 0.9188026736413833
- Precision score: 
  - high_risk: 0.04
  - low_risk: 1.00
  - macro avg: 0.52
  - weighted avg: 0.99
- Recall score:
  - high_risk: 0.71
  - low_risk: 0.92
  - macro avg: 0.82
  - weighted avg: 0.92

![image](https://user-images.githubusercontent.com/76754655/121603218-46ffa500-c9fd-11eb-9588-a208e86d795a.png)

![image](https://user-images.githubusercontent.com/76754655/121603250-5121a380-c9fd-11eb-9e72-f58f1e61b231.png)

![image](https://user-images.githubusercontent.com/76754655/121603268-58e14800-c9fd-11eb-9420-3d24fe95582c.png)

Easy Ensemble AdaBoost Classifier:

- Balanced accuracy score: 0.9445510026155187
- Precision score: 
  - high_risk: 0.08
  - low_risk: 1.00
  - macro avg: 0.54
  - weighted avg: 0.99
- Recall score:
  - high_risk: 0.91
  - low_risk: 0.94
  - macro avg: 0.93
  - weighted avg: 0.94

![image](https://user-images.githubusercontent.com/76754655/121603320-6dbddb80-c9fd-11eb-81bc-d74a10782e50.png)

![image](https://user-images.githubusercontent.com/76754655/121603345-77474380-c9fd-11eb-8cba-97626cb0184b.png)

![image](https://user-images.githubusercontent.com/76754655/121603361-7dd5bb00-c9fd-11eb-9f24-b75fdbdba447.png)

- As shown above, the balanced accuracy score of the Easy Ensemble AdaBoost Classifier was the highest at around 0.945
- The average precision was 0.99 for all six machine learning models with the Easy Ensemble AdaBoost Classifier with the highest high-risk precision of 0.08
- The recall score of the Easy Ensemble AdaBoost Classifier was the highest weighted average at 0.94

## Summary

As a summary, all of the six machine learning models had a high average precision of 0.99. The Easy Ensemble AdaBoost Classifier is recommended to be used based on the highest balanced accuracy score at around 0.945, the highest high-risk precision of 0.08, and the highest average weighted recall score of 0.94. 
