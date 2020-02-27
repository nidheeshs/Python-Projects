#Adult income census prediction using Logistic Regression

##Description
   There are 32561 instances and 15 columns in the dataset including dependent variable.
   In this project, I am working through the Income Prediction problem associated with the Adult Income Census dataset. The goal is to accurately predict whether or not someone is making more or less than $50,000 a year.

###Data Source- https://www.kaggle.com/uciml/adult-census-income

Libraries Used :


1. Numpy
2. Pandas
3. Matplotlib
4. Seaborn
5. Scipy
6. Sklearn

Steps:
1. Importing Data
2. Handling missing values
3. EDA using visualization
4. Creating dummy variables for categorical variable
5. Splitting data into Train and Test 
6. Model Selection
7. Model Validation

Exploratory Data analysis

Encode dependent variable , ie income to 0 and 1.
Insights:
*People with income <50K is larger than people with income >50K.
*Higher the value of eduction_num ,higher the probability of income greater than 50k
*Most of the people are from USA so we can drop column 'native.country'.
*Relationship and marital status gives us same information.

After checking Corelation heat map we can find following

*Education and education_num are corelated
*marital.status and realtionship are corelated 

Hence we can drop reltionship and education

Create dummies for workclass, marital.status, race, sex.
Concatenate X with other dataframes like marital_num, sex, workclass_num.    

