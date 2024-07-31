# deep-learning-challenge
Module 21 Challenge

## Overview of the Analysis

The purpose of this analysis is to build and optimize a deep learning model to predict the success of charity funding applications. Using machine learning and neural networks, this challenge aims to develop a binary classifier that predicts whether a funding application will be successful or not, with a goal of achieving a predictive accuracy of 75% or higher.

The dataset provided by the charity company contains over 34,000 records of organizations that have received funding. The dataset includes various columns capturing metadata about each organization, such as application type, affiliation, classification, use case, organization, status, income amount, special considerations, ask amount, and whether the funding was successful.

## Results
* Data Preprocessing
    * Target Variable: IS_SUCCESSFUL
    * Feature Variables: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT
    * Removed Variables: EIN, or NAME
        * These columns were removed as they are identifiers and do not contribute to the predictive power of the model.
     
  
* Compiling, Training, and Evaluating the Model
    * First Attempt
        * Neurons:
        * Layers: 2 hidden layers
        * Activation Functions
        * Result: 73%
        * Achived the target model performance?: 
    * Second Attempt
        * Changes: Dropped the following columns: EIN, NAME, and SPECIAL_CONSIDERATIONS
              * more 
        * Result: 71%
        * Did the attempts increase model performance?: No

## Summary

The initial neural network model achieved a training accuracy of around 73% and a test accuracy of 72%. The target accuracy of higher than 75% was not met. However, the model can be used for further improvements. The overall result is that the model can moderately predict the success of funding applicants.

Recommendations for further optimization include increasing the model complexity by adding more layers and neurons. Further experiments can be conducted by removing some columns or generating new ones. Additionally, trying different activation functions might help. By implementing these changes, the model's performance can potentially be improved to achieve higher accuracy. Exploring other machine learning models could also be beneficial for this prediction.
