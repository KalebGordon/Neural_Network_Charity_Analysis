# Neural_Network_Charity_Analysis

## Overview
Using our knowledge of TensorFlow, will design a neural network or deep learning model that creates a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. 

## Results

# Data Preprocessing
What variable(s) are considered the target(s) for your model?
- The target variable is whether or not the organization is successful. 

What variable(s) are considered to be the features for your model?
- Every variable that is not the 'IS_SUCCESSFUL' variable is considered a feature. These include ASK_AMT, APPLICATION_TYPE, STATUS, INCOME_AMT, and SPECIAL_CONSIDERATIONS. 

What variable(s) are neither targets nor features, and should be removed from the input data?
- The EIN and NAME variables are unique individual identifiers, and are not relevant to this analysis.

# Compiling, Training, and Evaluation
How many neurons, layers, and activation functions did you select for your neural network model, and why?
- For my first attempt, I used two hidden layers, with the first containing 102 neurons and the second containing 52 neurons. The activation function I chose was ReLu. This was different than my original attempt because I changed the replaced values from under 500 to under 250. 

- For my second attempt, I used two hidden layers, with the first containing 154 neurons, and the second containing 102 neurons. The activation function I chose was ReLu. This attempt used more neurons. 

- For my third attempt, I used three hidden layers, with the first containing 102 neurons, the second containing 52 neurons, and the third containing 21 neurons. The activation function I used was ReLu. This attempt contained more layers. 

Were you able to achieve the target model performance?
- I was unable to reach the target model performance of 75%. The closest any of my models got was 73.20%, which I achieved on my first attempt at optimization.

What steps did you take to try and increase model performance?
- I was thinking that increasing the amount of layers and decreasing the neurons in the second and third layer would narrow down the model and increase accuracy. Unfortunately that was not the case. I attempted using other activation functions as well in other attempts, this did not help. 

## Summary
The neural network model did not reach the target accuracy of 75%, and was a little under 2% off. The target is very close to our reported accuracy. I would suggest cleaning the dataset more to remove potential outliers, in addition to considering a model such as Random Forest Classifier.
