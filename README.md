## Overview
The purpose of this project was to use several different machine learning models to analyze a dataset from credit card company LendingClub.  The goal was to evaluate credit risk and also, by comparing the different models, make a determination about which model is best suited to the task.  The dataset was imported, pre-processed, and then run through the Random Over Sampler, SMOTE, Cluster Centroids, SMOTEENN, Balanced Random Forest Classifier, and Easy Ensemble AdaBoost Classifier algorithms.

## Results 
**Random Oversampling**
The results of the Random Oversampling show better recall than precision, but neither is well-balanced.
- Balanced Accuracy Score: 58%
- Precision: 	
  - High Risk: .01 
  - Low Risk: 1.0
- Recall: 	
  - High Risk: .46 
  - Low Risk: .69
  
  ![ROS.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/ROS.PNG)

**SMOTE**
The results of the SMOTE algorithm show better recall than precision but neither is well balanced.
- Balanced Accuracy Score: 65%
- Precision: 	
  - High Risk: .01
  - Low Risk: 1.0
- Recall: 	
  - High Risk: .56 
  - Low Risk: .73

![smote.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/smote.PNG)

**Cluster Centroids**
The results of the Cluster Centroids algorithm show better recall than precision but is not well balanced.
- Balanced Accuracy Score: 65%
- Precision: 	
  - High Risk: .01 
  - Low Risk: .99
- Recall: 	
  - High Risk: .51 
  - Low Risk: .56

![cc.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/cc.PNG)

**SMOTEENN**
The results of the SMOTEEN algorithm show better recall than precision but is not well balanced.
- Balanced Accuracy Score: 53%
- Precision: 	
  - High Risk: .01 
  - Low Risk: 1.0
- Recall: 	
  - High Risk: .73 
  - Low Risk: .58

![smoteenn.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/smoteenn.PNG)

**Balanced Random Forest**
The results of the Balanced Forest algorithm show better recall than precison
- Balanced Accuracy Score: 77%
- Precision: 
  - High Risk: .03 
  - Low Risk: 1.0
- Recall: 
  - High Risk: .66 
  - Low Risk: .88
  
  ![brf.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/brf.PNG)

**Easy AdaBoost**
- Balanced Accuracy Score: 92%
- Precision: 
  - High Risk: .09 
  - Low Risk: 1.0
- Recall: 
  - High Risk: .89 
  - Low Risk: .94

![eea.PNG](https://github.com/Alawler12/Credit_Risk_Analysis/blob/main/screenshots/eea.PNG)
Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
