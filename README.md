# Goodrich_N_CS4200_Assignment_2

For this project, I created two different models to predict future covid cases. For the project, I borrowed data from the following site, and only used data for covid cases in the United States: https://github.com/owid/covid-19-data

1. Linear Regression

  For this part, I used a basic linear regression model that looked at the previous trends of covid cases, and then made predictions about the future trends for the following 25 days.
  
  I have two different graphs that were created to represent these trends: the first one used a Decision Tree Regression model and the second uses the Linear Regression model. The linear regression model seemed to provide the most plausible results since the decision tree saw an uncharacteristic rise in covid cases early on before normalizing.
  
2. Decision Tree

  For this part, I manipulated the data significantly to create a model that predicted not necessarily the number of cases, but the severity of cases.
  
  The data looks at the following factors: 'new_cases', 'rep_rate', 'new_tests', 'pos_rate', 'tests_per_case', 'new_vac'
  
  The data for the new_cases are actually rated on a scale of 1-5 based off the number of cases (similar to new_tests, and new_vac which is on a scale of 1-7). These scales allowed for my model to give more accurate results when the tree compiled.

   The two models tsearched the trees at a max-depth of 5. Two decision trees were creating using a different criterion for each: gini and entropy.
