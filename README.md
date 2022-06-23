# Neural_Network_Charity_Analysis

## Overview
The purpose of this analysis is to use machine learning and neural networks with the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful is funded by Alphabet Soup. 

## Results

### Data Preprocessing
* Target variable that identifies whether the charity donation was used effectively
  * Column IS_SUCCESSFUL
* Feature variables:
  * APPLICATION_TYPE
  * AFFILIATION
  * CLASSIFICATION
  * USE_CASE
  * ORGANIZATION
  * STATUS
  * INCOME_AMT
  * SPECIAL_CONSIDERATIONS
  * ASK_AMT
* Variables that are neither targets nor features, and should be removed from the input data
  * Columns with identification information: 
    * EIN
    * NAME

### Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
* This neural model is based on two hidden layers
  * 1 layer with 80 neurons
  * 1 layer with 30 neurons
* Input data 
  * 43 features
  * 25,724 samples
* Output layer
  * Binary classification
    * Consists of a unique neuron
    * Sigmoid is used for this layer
* Training process
  * Utilized the activation functionality of ReLU for the 2 hidden layers
* Model accuracy
  * Approximately 75%
  * Did not satisfy the target model performance 
    * Did not help to predict the outcome of charity donations
  * Increase target model performance
    * None of the following steps helped to improve target model performance 
      * Applied bucketing to ASK_AMT feature
      * Re-organized values by intervals
      * Increased the number of neurons on 1 of the 2 hidden layers
      * Added a model with 3 hidden layers
      * Used a different activation function

## Summary
In terms of accuracy, the neural network model only reached approximately 75%. For this reason, the model is not considered to be outperforming. As this is considered to be a binary classification scenario, additional steps could be as follows: 
* Use a supervised machine learning model
  * Random Forest Classifier model 
    * This model might have heightened accuracy and efficiency by combining a multitude of decision trees
    * Goal would be to generate a classified output that could then be used to evaluate performance
