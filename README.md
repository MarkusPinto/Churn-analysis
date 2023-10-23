## Final Project Submission

Please fill out:
* Student name: Mark Bundi
* Student pace:  part time 
* Scheduled project review date/time: 
* Instructor name: 
* Blog post URL: 

## Business Problem

The bussines problem in this senario is to provide Telecom company a prediction of churn of customers so it can effectively focus a customer retention marketing program.
Customer churn is the loss of clients or customers

## Data Understanding
The dataset contains data on the customers of a Telecom company. Each row represents a customer and the columns contain customer’s attributes which are described in the following:

state: the state the user lives in
account length: the number of days the user has this account
area code: the code of the area the user lives in
phone number: the phone number of the user
international plan: true if the user has the international plan, otherwise false
voice mail plan: true if the user has the voice mail plan, otherwise false
number vmail messages: the number of voice mail messages the user has sent
total day minutes: total number of minutes the user has been in calls during the day
total day calls: total number of calls the user has done during the day
total day charge: total amount of money the user was charged by the Telecom company for calls during the day
total eve minutes: total number of minutes the user has been in calls during the evening
total eve calls: total number of calls the user has done during the evening
total eve charge: total amount of money the user was charged by the Telecom company for calls during the evening
total night minutes: total number of minutes the user has been in calls during the night
total night calls: total number of calls the user has done during the night
total night charge: total amount of money the user was charged by the Telecom company for calls during the night
total intl minutes: total number of minutes the user has been in international calls
total intl calls: total number of international calls the user has done
total intl charge: total amount of money the user was charged by the Telecom company for international calls
customer service calls: number of customer service calls the user has done
churn: true if the user terminated the contract, otherwise false

## IMPORTED LIBRARIES

The following Python Libraries were imported and utilised in the  projects: 

- pandas
- numpy
- matplotlib.pyplot
- seaborn as sns
- sklearn.linear_model import LogisticRegression
- sklearn.preprocessing import StandardScaler
- sklearn.preprocessing import OneHotEncoder
- sklearn.tree import DecisionTreeClassifier
- sklearn.metrics import accuracy_score
- sklearn.neighbors import KNeighborsClassifier

### Summary of data


## Data Preparation

Categorical data such state,international plan and voice mail plan have to be converted to numerical form.

The data is scalled using the standard scaler to balance the impact of all variables on the distance calculation and can help to improve the performance of the algorithm

The column phone number was dropped since it is a unique identifier and has no impact on the churn of customers

### Baseline Model
The baseline model is a simple model  used to contextualize the results of trained models. We create the basiline model to provide a reference point for measuring the performance of other models.
The baseline model chosen is a Logistical regression model

### Observations
The accuracy of the models was:

Logistical regression : 86%

Decision Tree : 91.8%

KNN Classifier: 90.6%

## Conclusion 
Our goal was to identify clients which are likely to churn, so we can do special-purpose marketing strategies to avoid the churn event. For this we evaluated differently preprocessed datasets and different classifiers.
In the classification chapter we have trained several different classifiers, including a Logistic Regression, a K-Nearest Neighbors Classifier and Decision Tree.

## Recomendations
The decision tree model has the highest accuracy in predicting customer churn. This information will be useful in targeted markrting towards clients.