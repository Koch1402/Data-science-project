# Data-science-project

## Introduction

My group consists of Jonathan Low, Neo Yu Hui, and Jerick Ho. Our SC1015 data science project is on using machine learning to predict the success and severity of terrorist attacks. Using various models, we will use a few variables that could be attained before an attack through intelligence gathering, and using those variables to predict the likelihood of success and the number of fatalities if the attack were to occur.

## Problem Statement
What makes terrorist attacks successful?​

### Goal
To use machine learning and past data to train models to determine the level of resources needed to recover from terrorist attacks.

## Data set

Our data set is from Kaggle [https://www.kaggle.com/datasets/START-UMD/gtd/data]. It is an open-source database of terrorist attacks that have happened from 1970 to 2017. The database is maintained by researchers at the National Consortium for the Study of Terrorism and Responses to Terrorism (START), headquartered at the University of Maryland. It contains more than 180,000 terrorist attacks, both successful and failed attacks. Each attack records more than 100 variables or both categorical and numerical data, from these attacks, such as location, perpetrator, casualties, etc.

## EDA
Our EDA focuses on identifying trends in the data. We focused on the data points that would be relevant to our problem statement, such as attack type, success distribution, and more.

## Analysis outcomes
We used feature importance to identify important features in determining success. From the top of the list of variables, we eliminated certain variables from logical deduction as we wanted to only use variables that would be available after an attack has occurred such as nkill, or wound.

## Models

We aimed to create a model that could be used to predict the likelihood of success of an attack from data points that could be collected before an attack. Subsequently, we would use these data points to predict the number of fatalities if the attack were to be carried out. To do this, we had to narrow down the >100 data points to find out which was more important in determining the success of an attack. To do this we used gradient boosting to rank the importance of variables for the success of an attack. We would also use our discretion to determine if this data could be collected before an attack (eg, you would only know the number killed after an attack was successful, while it is of high importance we cannot use it for our model). Using our chosen variables we performed trained 3 models, logistic regression, Gradient Boosting, and Multi-Layer Perceptron (MLP), and compared their prediction accuracy. Using our results from these models, we proceeded to predict nkill (number killed) using the predicted success. To do this we used 3 models, random forest regressor, Gradient Boosting, and MLP.  

## Conclusion
The most accurate out of the 3 models that we tested in predicting success was Gradient Boosting, followed by MLP and Logistic Regression. For predicting nkill, the best accuracy was Random forest regressor, followed by Gradient Boosting and MLP. Additionally, we trained a model with and without success as a possible variable, and found that with success as a variable, there was a slight improvement

Linking back to our goal, our model was able to predict success and subsequently nkill with accuracy, given a set of variables that could conceivably be acquired through intelligence services in real life. Knowing the possibility of success and possible number killed from an attack can help experts to determine the level of resources that are needed to recover from terrorist attacks. 

Possible future improvements could include training another model to predict the property damage that could be caused by a terrorist attack, as this also affects the resources needed. 
