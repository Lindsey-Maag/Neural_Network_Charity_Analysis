# Neural_Network_Charity_Analysis

## Overview
Use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results
- Data Preprocessing
  - What variable(s) are considered the target(s) for your model?
    - The "IS_SUCCESSFUL" column is the target variable which contains binary information showing whether or not funding that was provided by Alphabet Soup was was used effectively 
  - What variable(s) are neither targets nor features, and should be removed from the input data?
    - Columns "EIN" and "NAME" were dropped as the indentifying information contained was not critical for analysis 
  - What variable(s) are considered to be the features for your model?
    - All remaining columns are considered to be features: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT"

- Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
    -  
  - Were you able to achieve the target model performance?
    - I was not able to acheive the target model. 
    - Original Model:
    - ![ORIG](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/accuracy.PNG)
    - Optimization Attempt 1
    - ![OPT1](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/accuracy_opt1.PNG)
    - Optimization Attempt 3
    - ![OPT2](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/accuracy_opt2.PNG)
    - Optimization Attempt 
    - ![OPT3](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/accuracy_opt3.PNG)
  - What steps did you take to try and increase model performance?
    - 

## Summary
(include a recomendation)
