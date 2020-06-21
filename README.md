# Passenger Satisfaction Predictor

## Introduction
Classifying customers who are satisified and dissatisfied with the services of a company is very helpful in devleoping focused marketing and user retention strategies. 

In a sector like air travel where there are structured rewards programs for customer retention, such classifications gain increased signifcance.

Here we are trying to build a model for classifying satisfied and dissatisfied customers of an airline company.

## Data Description
The dataset contains 23 features which includes some demographic information, flight information like class of travel, flight distance, delays etc. and some ratings the customer gave for inflight services. It also provides information on customers whether these passengers were satisfied with the service or dissatisfied.

The dataset contains records of 103904 passengers. The dataset had some missing data and it had to be taken care of during the analysis. 

The dataset was more or less balanced with 9:11 ratio for satisfied and dissatisfied customers.

![Count Plot](https://github.com/muhammedsalihk/Passenger-Satisfaction-Predictor/blob/master/Images/Image%201.png)

## Methodology
A detailed exploratory analysis was perfomed on the data and based on the inferences obtained, a set of relevant features were selected and some new features were engineered.

![EDA Sample](https://github.com/muhammedsalihk/Passenger-Satisfaction-Predictor/blob/master/Images/Image%202.png)

The data was divided into two sets (train and test) in an 80-20 ratio. the hyperparameters were tuned based on a 4 fold cross validation approach using sklearn’s GridSearchCV. Finally, the performance of the different models with the tuned set of hyperparameters were evaluated on the test set.

The evaluation metric used for determining the performance of the models was Accuracy Score. 

## Results
The following models were evaluated for performance on each of the three sampling techniques.

    1. Logistic Regression
    2. K Nearest Neighbours
    3. Decision Tree
    4. Random Forest
    5. Gradient Boosting
    6. XGBoost Classifier
    7. XG Boost Random Forest Classifier

The performance of the different models are summarised below.

![Results](https://github.com/muhammedsalihk/Passenger-Satisfaction-Predictor/blob/master/Images/Results.png)

The **XGBoost Classifier** performed the best giving an **accuaracy score of 0.965**
