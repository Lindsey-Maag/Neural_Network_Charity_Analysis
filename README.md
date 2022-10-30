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
    -  Original Layers:
    - ![Orig](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/layers.PNG)
    - Optimization Attempt 2 & 3:
    - ![Opt23](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/layers2.PNG)
    - I added an additional hidden layer in 2 of my optimization attempts. The original design had 80 neurons in the first layer and 30 in the second. I used 200 neurons in the first layer, 50 neurons in the second, and added a third layer with 10 neurons. The original design had 5,981 parameters and with added neurons and layers the parameters increased to 18,771. Althought this would sacrifice speed my attempt was to increase accuracy of the model.
  - Were you able to achieve the target model performance?
    - I was not able to acheive the target model. 
    - Original Model:
    - ![ORIG](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/accuracy.PNG)
    - Optimization Attempt 1
    - ![OPT1](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/accuracy_opt1.PNG)
    - Optimization Attempt 2
    - ![OPT2](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/accuracy_opt2.PNG)
    - Optimization Attempt 3
    - ![OPT3](https://github.com/Lindsey-Maag/Neural_Network_Charity_Analysis/blob/main/Images/accuracy_opt3.PNG)
  - What steps did you take to try and increase model performance?
    - My first attempt at optimization I focused on noisy variables. I increased the binning of "APPLICATION_TYPE" from a threshold of 400 for the 'other' category to 1000.
    - My second attempt focused on adding an additional hidden layer and additional neurons.
    - My third attempts focused on changing activations in the second and third hidden from "relu" to "tanh" and also changing the optimizer from "adam" to "RMSprop".

## Summary
(include a recomendation)
