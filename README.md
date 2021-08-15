# Credit Risk Analysis 

## Overview of the analysis: 
The purpose of this analysis is to solve the unbalanced classification problem in Credit risk where good loans are easily outnumbered by risky loans. Therefore, I have employed different techniques to train and evaluate models with unbalanced classes.


## Tools 
- Jupyter notebook - imbalanced-learn and Scikit-learn libraries


## Results:
Below is the list of the balanced accuracy scores, the precision and recall scores of all six machine learning models : 

- Naive Random Oversampling: the balance accuracy score - 0.6547385707934685


![Picture](https://user-images.githubusercontent.com/79213116/129494882-593f2b32-7fac-425e-a4d8-f246dea2767f.png)


- SMOTE Oversampling: the balance accuracy score - 0.66201409663885 


![](https://user-images.githubusercontent.com/79213116/129494884-dbac5e6a-3951-4f39-a193-f085601e10eb.png)


- ClusterCentroids undersampling: the balance accuracy score - 0.5439153831192286



![](https://user-images.githubusercontent.com/79213116/129494883-41e4b15a-d896-4b12-bb84-fccc084d337a.png)


- SMOTEENN: the balance accuracy score - 0.6472841741611017
 
![](https://user-images.githubusercontent.com/79213116/129494885-1c27b195-b099-4062-ad55-bf5953f365d0.png)





## Summary: 




The precision for high_risk is low in all the models. This indicates that there are more high_risk false positives. Therefore, this model will potnetially identify low-risk individual as high_risk. 

The recall is high for both high-risk and low_risk, which indicates that the model will identify all the correct individuals for high risk and low_risk, except for the ClusterCentroid classification model as the recall for high_risk is low.

In this case, recall is more important than precision as it is better to have more False Positives then to have less False Negatives, in other words it is safer to identify low_risk individuals as hig_risk compared to identifying indivuals which are high_risk as low_risk.















