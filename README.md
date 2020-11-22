## Overview
The purpose of this project was to use several different machine learning models to analyze a dataset from credit card company LendingClub.  The goal was to evaluate credit risk and also, by comparing the different models, make a determination about which model is best suited to the task.  The dataset was imported, pre-processed, and then run through the Random Over Sampler, SMOTE, Cluster Centroids, SMOTEENN, Balanced Random Forest Classifier, and Easy Ensemble AdaBoost Classifier algorithms.

## Results 
**Random Oversampling**
The results of the Random Oversampling show better recall than precision, but neither is well-balanced between High and Low risk.  And the accuracy score is pretty poor at 58%.
- Balanced Accuracy Score: 58%
- Precision: 	
  - High Risk: .01 
  - Low Risk: 1.0
- Recall: 	
  - High Risk: .46 
  - Low Risk: .69
  
  ![ROS.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/ROS.PNG)

**SMOTE**
The results of the SMOTE algorithm show a better accuracy score than ROS but it's still a failing grade at 65%.  There is better recall than precision but neither is well balanced between High and Low risk.
- Balanced Accuracy Score: 65%
- Precision: 	
  - High Risk: .01
  - Low Risk: 1.0
- Recall: 	
  - High Risk: .56 
  - Low Risk: .73

![smote.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/smote.PNG)

**Cluster Centroids**
The results of the Cluster Centroids show an unimproved accuracy scrore.  The algorithm shows better recall than precision, with more balance in Recall then Precision.
- Balanced Accuracy Score: 65%
- Precision: 	
  - High Risk: .01 
  - Low Risk: .99
- Recall: 	
  - High Risk: .51 
  - Low Risk: .56

![cc.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/cc.PNG)

**SMOTEENN**
The results of the SMOTEEN algorithm show the worst accuracy score out of the six models at 53%.  There is better recall than precision but is still not well balanced.
- Balanced Accuracy Score: 53%
- Precision: 	
  - High Risk: .01 
  - Low Risk: 1.0
- Recall: 	
  - High Risk: .73 
  - Low Risk: .58

![smoteenn.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/smoteenn.PNG)

**Balanced Random Forest**
The results of the Balanced Forest algorithm show an improving accuracy score at 77%.  There is better recall than precison, and balance is getting closer.
- Balanced Accuracy Score: 77%
- Precision: 
  - High Risk: .03 
  - Low Risk: 1.0
- Recall: 
  - High Risk: .66 
  - Low Risk: .88
  
  ![brf.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/brf.PNG)

**Easy AdaBoost**
The results of the Easy Adaboost algorithm shows the best accuracy score by far at 92%.  The model shows better recall than precision, and there is a better balance between High and Low risk loans.
- Balanced Accuracy Score: 92%
- Precision: 
  - High Risk: .09 
  - Low Risk: 1.0
- Recall: 
  - High Risk: .89 
  - Low Risk: .94

![eea.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/eea.PNG)

### Summary: 
A comparison of these six models shows that the Adaboost Ensemble Classifier performs the best.  In addition to having the best balanced accuracy score at 92%, this model also shows very good recall at an average of 94%.  The recall for High Risk loans is 89% and for Low Risk loans is 94%.  This model has very good precision for Low Risk loans, at 100%, but only 9% precision for High Risk loans.  This all shows that this model is very specific and will do a very good job of finding the loans in each category, but that the accuracy of each characterization is better for Low Risk loans than High Risk loans.  In the case of a financial institution assessing credit risk, it is more important to be sensitive than precise, especially in regard to the riskiness of giving out loans.  It is better to err on the side of approving a low risk loan than a high risk loan, if the aim is to maintain the financial integrity of your institution.  In this case, the Adaboost Ensemble Classifier is a good algorithm for this task.

