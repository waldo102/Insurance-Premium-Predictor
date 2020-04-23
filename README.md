# Insurance-Premium-Predictor
Goal: Use customer demographic information to predict the charge amount for the monthly insurance premium

Data: insurance.csv
  * contains 7 variable and 1k observations

Files:
  * insurance_premium_predictor.ipynb - performs data cleaning, data preparation, data analysis, and also model specifications and hyperparameter tuning.
  
Models:
  * Linear Regression
  * Polynomial Regression
  * Decision Tree Regression
  * Random Forest Regression
  * Support Vector Regression

Performance Metrics:
  * Coefficient of Determination (R2)
  * Root Mean Square Error (RMSE)
  
Results:

The three models performed very similarily:

  * Linear Regression         : R2 = 0.72, RMSE = 14438 
  * Polynomial Regression     : R2 = 0.84, RMSE = 4328
  * Decision Tree Regression  : R2 = 0.85, RMSE = 4503
  * Random Forest Regression  : R2 = 0.86, RMSE = 4028
  * Support Vector Regression : R2 = 0.71, RMSE = 6467

Conclusions:

The Random Forest model edged out the other models in terms of accuracy. Typically, it is very difficult for models to perform well
with a limited amount of variables and observations. The models under consideration each performed well, but the Random Forest
was able to predict insurance premiums more precisely. For this task, the Random Forest regressor is the best model.

In addition, according to the data, the most important variables in determining insurance premiums are the following:

 1. Smoking Behavior
 2. Body Mass Index (BMI)
 3. Age
 
In the exploratory data analysis, it was clear whether the person smoked or not affects the charge amount of the insurance premium.
The BMI serves as a measure of a person's health, so it makes sense it would affect insurance premium charges.
Lastly, age is a classic determinant of the price of insurance. The importance of these variables in the model supports the adequacy of the 
Random Forest model in predicting insurance premiums.


For more details on the analysis of this project, please read and follow the analysis in the jupyter notebook file insurance_premium_predictor.ipynb 

*Resources: This project was part of Rajeev D. Ratan's course, Data Science & Deep Learning for Business™ 20 Case Studies as presented in udemy.com*
