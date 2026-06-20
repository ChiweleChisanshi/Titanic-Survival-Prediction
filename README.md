# Titanic Survival Prediction

## Overview

This project uses the Titanic passenger dataset to predict survival and analyze passenger patterns using logistic regression and linear regression.

The project looks at how features like passenger class, sex, age, fare, family size, and embarkation port relate to survival, passenger class, fare, and age.

## Tools Used

- Python
- pandas
- NumPy
- scikit-learn
- matplotlib
- seaborn
- Logistic Regression
- Linear Regression

## Dataset

The dataset includes information about Titanic passengers, such as:

- Passenger ID
- Survival status
- Passenger class
- Name
- Sex
- Age
- Number of siblings/spouses aboard
- Number of parents/children aboard
- Ticket number
- Fare
- Cabin
- Embarkation port

The dataset had 891 passenger records.

## Project Goals

The main goals of this project were to:

- Predict whether a passenger survived
- Predict passenger class
- Predict embarkation port
- Predict passenger fare
- Predict passenger age
- Evaluate how well each model performed

## Models Used

## 1. Survival Prediction

I used logistic regression to predict whether a passenger survived.

Features used:

- Passenger class
- Sex
- Age
- Fare

The model achieved about 80% accuracy.

The confusion matrix showed:

- 469 passengers were correctly predicted as not surviving
- 243 passengers were correctly predicted as surviving
- 80 passengers were incorrectly predicted as surviving
- 99 passengers were incorrectly predicted as not surviving

This model performed fairly well and showed that class, sex, age, and fare were useful for predicting survival.

## 2. Passenger Class Prediction

I used logistic regression to predict passenger class.

Features used:

- Fare
- Family size
- Age
- Embarkation port

The model achieved about 79% accuracy.

The model was better at predicting 1st class and 3rd class passengers, but had more difficulty with 2nd class passengers.

## 3. Embarkation Port Prediction

I used logistic regression to predict where passengers embarked.

Features used:

- Passenger class
- Fare
- Age
- Family size

The model achieved about 73% accuracy.

The embarkation ports were encoded as:

- 0 = Southampton
- 1 = Cherbourg
- 2 = Queenstown

The ROC curve showed that the model performed best for one port, but weaker for the others.

## 4. Fare Prediction

I used linear regression to predict passenger fare.

Features used:

- Passenger class
- Age
- Family size
- Embarkation port

Results:

- Mean Squared Error: 1530.48
- Root Mean Squared Error: 39.12
- R-squared: 0.379

The model had moderate performance. It explained some of the variation in fare, but other important factors were likely missing.

## 5. Age Prediction

I used linear regression to predict passenger age.

Features used:

- Passenger class
- Fare
- Family size
- Embarkation port

Results:

- Mean Squared Error: 140.99
- Root Mean Squared Error: 11.87
- R-squared: 0.167

This model did not perform very well. The features used were not strong predictors of age.

## Visualizations

The project includes:

- Confusion matrix for survival prediction
- Confusion matrix for passenger class prediction
- ROC curve for embarkation port prediction
- Actual vs. predicted fare plot
- Actual vs. predicted age plot

## Key Findings

- Survival was strongly related to passenger class, sex, age, and fare.
- The survival model had the best performance, with about 80% accuracy.
- Passenger class was also predicted fairly well, with about 79% accuracy.
- Embarkation port prediction was moderate, with about 73% accuracy.
- Fare prediction had moderate results.
- Age prediction was weak because the selected features did not explain much of the variation in age.

## Skills Demonstrated

- Python programming
- Data analysis
- Logistic regression
- Linear regression
- Machine learning basics
- Feature engineering
- Model evaluation
- Confusion matrix interpretation
- ROC curve interpretation
- Data visualization

## What I Learned

This project helped me understand the difference between classification and regression models.

I learned that logistic regression is useful for predicting categories, such as survival or passenger class. I also learned that linear regression is used for predicting numbers, such as fare or age.

I also learned that model performance depends heavily on the features used. Some outcomes, like survival, were easier to predict because the features were closely related to the target. Other outcomes, like age, were harder to predict because the available features were not strong enough.


## Future Improvements

In the future, I would improve this project by:

- Splitting the data into training and testing sets
- Handling missing values more carefully
- Adding more feature engineering
- Comparing logistic regression with other models
- Using precision, recall, and F1-score
- Creating cleaner visualizations

## Conclusion

This project gave me hands-on practice with predictive analytics and machine learning. The strongest model was the survival prediction model, which achieved about 80% accuracy. The project helped me understand how to build, evaluate, and interpret basic machine learning models.
