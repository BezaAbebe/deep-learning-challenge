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
        * First Hidden Layer: 100 neurons
        * Second Hidden Layer: 50 neurons
        * Two hidden Layers
        * one output layer
        * Activation Functions:
             * ReLU for hidden layers (introduces non-linearity and helps in learning complex patterns)
             * Sigmoid for output layer (outputs probabilities for binary classification)
             * The reason ReLu activation function is used is because it is the most commenly used for                     hidden layers and it helps the model learn complex model. In additon the reason why the                    Sigmoid activation funditon in the output layer is used because it is very suitable for                      binary classification as its outcome probabilitis are between 0 and 1.
         * Target Model Performance:
            * Test Loss: 0.5726
            * Test Accuracy: 0.7283
            * The target model performance of achieving higher than 75% accuracy was not met.
        * Steps Taken to Optimize Model Performance:
               * Dropped unnecessary columns: EIN, NAME, and SPECIAL_CONSIDERATIONS.
               * Increased the cutoff value and created a list of application types to be replaced, changing from 500 to 5000.
               * Used the Affiliation variable name for classification to replace.
               * The target model performance of achieving higher than 75% accuracy was not met in this optimization attempt.
          
          


## Summary

The initial neural network model achieved a training accuracy of around 73% and a test accuracy of 72%. The target accuracy of higher than 75% was not met. However, the model can be used for further improvements. The overall result is that the model can moderately predict the success of funding applicants.

Recommendations for further optimization include increasing the model complexity by adding more layers and neurons. Further experiments can be conducted by removing some columns or generating new ones. Additionally, trying different activation functions might help. By implementing these changes, the model's performance can potentially be improved to achieve higher accuracy. Exploring other machine learning models could also be beneficial for this prediction.
