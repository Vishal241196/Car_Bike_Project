# Project Summary

- The Data science project which is given here is an analysis of Customer Churn. The purpose of this project is to predict the customer churn from each feature of their data such as Day Mins, Day Charge, Eve Mins, Eve Charge, Night Mins, International Mins, International Calls, International Charge, CustServ Calls, International Plan. The Goal and Insights of the project as follows,
  1. A trained model which can predict customer churn based on factors as inputs.
  

- The given data of churn has the 4617 data to perform a higher level machine learning where it is well structured. The features present in the data are 21 in total. The Shape of the data is 4617x21. The 21 features are classified into quantitative and qualitative where 5 features are qualitative and 16 features are quantitative.

- The dataset is a complete labelled data and categorical which decides the machine learning algorithm to be used. The important aspects of the data are depending on the correlation of data between features and Churn. The analysis of the project has gone through the stage of distribution analysis, correlation analysis and analysis by each department to satisfy the project goal.

- The machine learning model which is used in this project is Random Forest classifier which predicted the nearby higher accuracy of 93% to 97%. Since it is categorical labelled data, it has to go through the classifier machine learning techniques which will be suitable for this structured data. The numerical features are the most relevant in the model according to correlation technique.

### 1. Requirement
The data was given from the No-Churn Telecom for this project where the collected source is No-Churn Telecom. It is one of the leading data analytics and automation solutions. The data is not from the real organization. The whole project was done in Jupiter notebook with python platform.

### 2. Analysis
Data were analyzed by describing the features present in the data. the features play the bigger part in the analysis. the features tell the relation between the dependent and independent variables. Pandas also help to describe the datasets answering following questions early in our project. The futures present in the data are divided into numerical and categorical data.

##### Categorical Features
These values classify the samples into sets of similar samples. Within categorical features are the values nominal, ordinal, ratio, or interval based. The categorical features as follows,
- State
- Phone
- International Plan
- VMail Plan
- Churn

##### Numerical Features
These values change from sample to sample. Within numerical features are the values discrete, continuous, or timeseries based. The Numerical Features as follows,
- Account Length        
- Area Code
- VMail Message           
- Day Mins              
- Day Calls               
- Day Charge            
- Eve Mins              
- Eve Calls               
- Eve Charge            
- Night Mins            
- Night Calls             
- Night Charge          
- International Mins    
- International Calls     
- International Charge  
- CustServ Calls

##### Alphanumeric Features
Numerical, alphanumeric data within same feature. These are candidates for correcting goal.No alphanumeric data type is present in dataset.

##### Data Clean Check
The Data cleaning and wrangling is the part of the Data science project where the workflow the project go through this stage. because the damaged and missing data will lead to the disaster in the accuracy and quality of the model. If the data is already structured and cleaned, there is no need for the data cleaning. In this case, the given data have some outliers, we dectected and treated outliers by replacing with mean values of respective featuresand and make data cleaned and there are no missing data present in this data.

##### Analysis by Visualization
we can able to perform the analysis by the visualisation of the data in two forms here in this project. One is by distributing the data and visualize using the density plotting. The other one is nothing but the correlation method which will visualise the correlation heat map and we can able to achieve the correlation values between the numerical features.
1. Distribution Plot
   - In general, one of the first few steps in exploring the data would be to have a rough idea of how the features are distributed with one another. To do so, we shall invoke the familiar kdeplot function from the Seaborn plotting library. The distribution has been done by both numerical and categorical features. it will show the overall idea about the density and majority of data present in a different level.

2. Correlation Plot
   - The next tool in a data explorer's arsenal is that of a correlation matrix. By plotting a correlation matrix, we have a very nice overview of how the features are related to one another. For a Pandas data frame, we can conveniently use the call .corr which by default provides the Pearson Correlation values of the columns pairwise in that data frame. The correlation works bet for numerical data where we are going to use all the numerical features present in the data.

From the above Pearson correlation heat plot, we can be to see that correlation between features with numerical values in the dataset. The heat signatures show the level of correlation from 0 to 1. from this distribution we can derive the facts as follows,
The most important features selected are Day Mins, Day Charge, Eve Mins, Eve Charge, Night Mins, International Mins, International Calls, International Charge, CustServ Calls, International Plan.

##### Machine Learning Model
The machine learning models used in this project is Random Forest classifier.

Both machine learning algorithms are best for classification and labelled data. The train and test data are divided and fitted into the model and passed through the machine learning. Since we have already noted the severe imbalance in the values within the target variable, we implement the SMOTE method in the dealing with this skewed value via the learn Python package. The predicted data and test data achieved the accuracy rate of 94.62% uaing Random Forest classifier.

From the above model,We select Random Forest classifier for fitting the model and than Evaluted the model.
In model Evalution part we calculate,
1. accuracy score
2. confusion matric
3. MSE and RMSE values
4. Precision
5. Recall
6. F1 score
7. Classification Report

### 3. Summary
The machine learning model has been fitted and predicted with the accuracy score. The goal of this project is nothing but the results from the analysis and machine learning model.

##### Goal 3: A trained model which can predict customer churn based on factors as inputs.
The trained model is created using the Random Forest classifier algorithm as follows, 
1. accuracy score is 94.62%
2. confusion matric 
                  
                  col_0   0    1   
                  Churn
                      0  1147  51   
                      1   77  1102   
                      
3. MSE value =  0.05384938998737905
4. RMSE value = 0.23205471334876834
5. Precision = 95.6%
6. Recall = 93.5%
7. F1 score = 94.5%
8. Classification Report
                       
                       precision  recall  f1-score   support

                   0       0.94      0.96      0.95      1198
                   1       0.96      0.93      0.95      1179
                   
            accuracy                           0.95      2377
           macro avg       0.95      0.95      0.95      2377
        weighted avg       0.95      0.95      0.95      2377
