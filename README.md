# Exploratory Data Analysis
## By Caleb Denzeil

# Dataset 1(Churn_Modelling.csv)
> The first dataset contains information about whether the bank customers or subscribers will discontinue a service or not
 and it's depicted as (1=yes or 0=no)
 
 # Dataset 2(insurance.csv)
 >The second dataset contains information about health insurance charges.A person is offered insurance depending on a number of factors like age, bmi or if the person is a smkoker or non-smoker.
 
 >I did some feature engineering and divided the age and bmi columns into different categories
 
 ## Summary of Findings(Dataset 1)
 
>Their is no relationship between age and Creditscore.

>Germany has the highest credit score

>7962 customers remained and 2037 customers exited. That's 79.63% and 20.37% of customers.
>More female customers have exited than males.

>Their is a weak relationship between Tenure and creditscore. Customers with higher credit score have more tenures.

>Their is a weak relationship between EstimatedSalary and Age. Younger customers have a higher Estimated salary compared to the older generation.
 
>After exploratory data analysis, I trained a logistic regression model using the churn dataset.

>The independent variables that I used were 'CreditScore', 'Age', 'Tenure', 'Number_of_Products', 'Has_credit_card', 'IsActiveMember' and the dependent variable was Exited.

>From the confusion Matrix the model the algorithm made 2311 true positive predictions (correctly predicted positive cases) and 83 false negative predictions (incorrectly predicted negative cases). It also made 68 false positive predictions (incorrectly predicted positive cases) and 538 true negative predictions (correctly predicted negative cases).

>The model preicted 80% of the outcome on the test data and 79% of the cases on the training data.
## Summary of Findings(Dataset 2)


>A majority of the smokers belong to the old_adults bracket and the young_adults are the least.

>Their is not that much of a relationship between age and bmi because their is a slight difference in their mean,older adults have a higher bmi compared to young adults.

>Females and males have almost the same bmi, although the male's bmi is higher seconded by females.

>The old adults are charged the most and the young adults the least.

>People with a higher bmi are charged more compared to those with less.

>Both smokers and non-smokers have almost the same bmi.

>I further trained a linear regression model with the insurance dataset. My independent variable age bmi and dependant charges.

>The training and set score are 0.1 and 0.06 which are relatively low meaning that the model is not a good fit.

>Due to the trainig and test sets perfoming not well the mean absolute error,mean squared error and root mean squared error were really high meaning that the model does not fit well with the dataset.