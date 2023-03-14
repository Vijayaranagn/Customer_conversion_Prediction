# Customer_conversion_Prediction

#Problem Statement

You are working for a new-age insurance company and employ multiple outreach plans to sell term insurance to your customers. Telephonic marketing campaigns still remain one of the most effective way to reach out to people however they incur a lot of cost. Hence, it is important to identify the customers that are most likely to convert beforehand so that they can be specifically targeted via call. We are given the historical marketing data of the insurance company and are required to build a ML model that will predict if a client will subscribe to the insurance. 

#Data

The historical sales data is available as a compressed file here. 

https://docs.google.com/spreadsheets/d/17MbVyO-sasOk0KswkdgEgOYdVES9JZyaIxOVQ1MZkLs/edit?usp=sharing

#Features

age (numeric)
job : type of job
marital : marital status
educational_qual : education status
call_type : contact communication type
day: last contact day of the month (numeric)
mon: last contact month of year
dur: last contact duration, in seconds (numeric)
num_calls: number of contacts performed during this campaign and for this client 
prev_outcome: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")
Output variable (desired target):
y - has the client subscribed to the insurance?

#Minimum Requirements:

It is not sufficient to just fit a model - the model must be analysed to find the important factors that contribute towards the price. 

AUROC must be used as a metric to evaluate the performance of the models.

Now we follow below steps to do this: 

1. IMPORT THE DATASET
2. CHECKING BALANCED OR NOT
3. DATA PREPROCESSING
4. CLEAN THE DATA
  
  A. First step is to check is there any missing value(data) & Duplicates data
  
  B. Second step is to check is data in right format
  
  C. Third step is to check is there any spelling mistakes in object datas:
  
  D. Fourth step is there any outliers in the given data

5. Exporatory Data Analysis (EDA)

Then we apply machine learning methods:

1. ENCODE THE DATA
  
  A. LABEL ENCODING
  
  B. ONE-HOT ENCODING
  
2. TARGET AND FEATURE SELCTION:

3. SPLITTING THE DATA
  
  A. Random Undersampling
  
  B. Random Oversampling

4. SMOTE
  A. SMOTEENN
  
Then we apply machine learning Algorithams:

1. Logistic Regression:

2. Decision Tree

3. KNN

4. XG_BOOST

5. Random Forest

SOLUTION STATEMENT:

MODELLING:

Models are tested to see which one can better predict consumer conversion.

LOGISTIC REGRESSION, the model AUROC score is 0.89
DECISION TREE, the model AUROC score is 0.77,
DECISION TREE with max depth, the model AUROC score is 0.87
KNN, the model AUROC score is 0.85
RANDOM FOREST, the model AUROC score is 0.90
XG BOOST CLASSIFIER, the model AUROC score is 0.9014
The model XG BOOST has the highest AUROC score, coming in at 0.914.

