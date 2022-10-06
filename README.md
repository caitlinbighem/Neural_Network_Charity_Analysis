# Neural_Network_Charity_Analysis

## Overview
The purpose of this analysis is to evaluate the impact of every donation and evaluate potential recipients. This helps to assure the foundations finances is being used effectively and efficiently. However, this is not always the case as, occasionally, an organization will collect the money and disappear. To minimize and/or prevent this outcome all together, we try to predict which organizations are worthy of donations and which can be viewed as high risk by using the data driven solution to anticipate these decisions with accuracy.

## Results

### Data Preprocessing
* **What variable(s) are considered the target(s) for the model?** 

The target is the "IS_SUCCESSFUL" because it consists of the data that determines whether the donations were used effectively. The target variable is the dependent variable, y.  

* **What variable(s) are considered to be the features for the model?** 

The variables below are considered to be the features for the model: 
    - APPLICATION_TYPE
    - AFFILIATION
    - CLASSIFICATION
    - USE_CASE
    - ORGANIZATION
    - STATUS
    - INCOME_AMT
    - SPECIAL_CONSIDERATIONS
    - ASK_AMT
These variables are the independent variables, x.

* **What variable(s) are neither targets nor features, and should be removed from the input data?** 

The identification columns EIN and NAME were dropped, as they do not contribute any useful information when completing the analysis.

### Compiling, Training, and Evaluating the Model
* **How many neurons, layers, and activation functions were selected for the neural network model, and why?** 

First Deep neural network model: 80 neurons were in the first hidden layer and 30 neurons were in the second hidden layer 
Second Deep neural network model: 100 neurons were in the first hidden layer, 30 neurons were in the second hidden layer and 10 neurons were in the third hidden layer.
An advantage for using the sigmoid activation function is that it identifies clear predictions from the input values. 

* **Was target model performance achieved?** 

Performance of 75% accuracy was not achieved by the target model, as it attained 79.25%. 

* **What steps were taken to try and increase model performance?** 

While trying to increase model performance, a third hidden layer was added with 10 neurons and the activation functions were updated. The first hidden layer retained the ReLU activation function, while the second and third layers adapted to the Sigmoid activation function. Unfortunately, these updates did not yeild a performance of 75%. 

## Summary
Regardless of the multiple attempts at optimizing the model, we did not reach a perfromance of 75%. However to increase the accuracy, we recommend adapting the number of hidden layers, neurons and the activation functions associated with each layer.