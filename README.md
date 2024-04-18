# Data-science-project

## Introduction

My group consists of Jonathan Low, Neo Yu Hui, and Jerick Ho. Our SC1015 data science project is on using machine learning to predict the success and severity of terrorist attacks. Using various models, we will use a few variables that could be attained before an attack through intelligence gathering, and using those variables to predict the likelihood of success and the number of fatalities if the attack were to occur.

## Data set

   Our data set is from Kaggle [https://www.kaggle.com/datasets/START-UMD/gtd/code]. It is an open-source database of terrorist attacks that have happened from 1970 to 2017. The database is maintained by researchers at the National Consortium for the Study of Terrorism and Responses to Terrorism (START), headquartered at the University of Maryland. It contains more than 180,000 terrorist attacks, both successful and failed attacks. Each attack records more than 100 variables or both categorical and numerical data, from these attacks, such as location, perpetrator, casualties, etc.

## EDA

## Our analysis

We aimed to create a model that could be used to predict the likelihood of success of an attack from data points that could be collected before an attack. Subsequently, we would use these data points to predict the number of fatalities if the attack were to be carried out. To do this, we had to narrow down the >100 data points to find out which was more important in determining the success of an attack. To do this we used gradient boosting to rank the importance of variables in respect to the success of an attack. We would also use our own discretion to determine if this data could be collected before an attack (eg, you would only know the number killed after an attack was successful, while it is of high importance we cannot use it for our model). Using our chosen variables we performed trained 3 models, logistic regression, Gradient Boosting, and Multi-Layer Perceptron (MLP), and compared their prediction accuracy. Using our results from these models, we proceeded to predict nkill (number killed) using the predicted success. To do this we used 4 models, random forest regressor, Gradient Boosting, MLP, and logistic regression.  

## Analysis outcomes

## Conclusion
