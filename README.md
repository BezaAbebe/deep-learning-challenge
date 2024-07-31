# deep-learning-challenge
Module 21 Challenge

## Overview of the Analysis

The purpose of this analysis is to build and optimize a deep learning model to predict the success of charity funding applications. Using machine learning and neural networks, this challenge aims to develop a binary classifier that predicts whether a funding application will be successful or not, with a goal of achieving a predictive accuracy of 75% or higher.

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
        * Did the attempts increase model performance?:



## Summary

Despite several optimization attempts, the model did not achieve the target performance of 75% accuracy. Future efforts could involve exploring other models like Random Forest, Gradient Boosting, or Support Vector Machines, which may be better suited for this classification problem.
