# Project Title : Credit-Card-Default-Prediction-Supervised-Machine-Learning-Classification-Capstone-Project
# Introduction
This project is aimed at predicting the case of customers default payments in Taiwan. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients.
# Steps Involved :
* Dataset Inspection
* EDA :
  1. Handling Missing Data
  2. Univariate Analysis
  
  ![image1](https://user-images.githubusercontent.com/93809665/229978595-460cb412-d6bb-4b82-8ea0-baca78680f2e.PNG)
  ![image2](https://user-images.githubusercontent.com/93809665/229978634-b8277aa3-a08e-4344-bb69-5f1bf59b7e08.PNG)
  ![image3](https://user-images.githubusercontent.com/93809665/229978672-defd52de-d692-4aad-9d4d-ebec2639d81d.PNG)
  

  3. Correlation
* One Hot Encoding
* Handling Class Imbalance : Using SMOTE
* Data Transformation
* Train Test Splitting
* Model Implementation
* Feature Importance On Random Forest Baseline Model
* Feature Importance On XG Boost Optimal Model

# Baseline Model Comparison Table
![image4](https://user-images.githubusercontent.com/93809665/229978715-9f95ee55-c300-4a99-8be7-5c3d2e125d8f.PNG)

# Optimal Model Comparison Table
![image5](https://user-images.githubusercontent.com/93809665/229978764-aa17445b-7da9-40ae-b563-952c60b0b32a.PNG)

# Conclusion :
After Basic EDA,
1. Limit amount was less for Credit Card Defaulters comparative to non defaulters.
2. Dataset have more females credit card holder,so number of defaulter have high proportion of females.
3. Credit Card No. of Defaulters as per education from top to bottom :
University>graduate school>High School>Others 
4. Number of defaulters have a higher proportion of Singles.

From all baseline models, Random Forest classifier shows highest test accuracy, F1 score and ROC score.

Baseline model of Random forest and decision tree shows huge difference in train and test accuracy which shows overfitting.

After cross validation and hyperparameter tuning, XG Boost shows highest test accuracy score of 88.10% and F1 Score is 0.875.

Thus XG Boost with optimal model is best to predict the credit Card Default

# Next Step :
* For Model Deployment we can use the Tuned XG BOOST Model. Where we suppose to make the prediction on monthly basis as per the previous records of customer and accordingly reject his/her credit request, if he/she is pretended to make default on his/her credit. 
