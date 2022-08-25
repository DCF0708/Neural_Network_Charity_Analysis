# Neural_Network_Charity_Analysis
The following analysis depicts the deployment and full optimization process of a Neural Network model. 
</br>
</br>

## Use Case: 
A non-profit organization specializes in the generation of funds for contribution to projects benefiting the ecosystem. An internal need has been identified, and the organization is now in search of a model that can give insight on the likelihood of success of future applicants. Data is provided for all past applicants. (see fig. 1)
</br>
</br>

![1](./Images/data1.png)
![2](./Images/data2.png)
</br>
</br>

The Neural Network (NN hencefourth) models implemented in this study are binary classifiers that return values signifying a positive prediction of success. The model will split the dataset and use part of the data to learn trends and feature correlations. The data not used in the learning stage is used to make predictions predictions of success using the learned trends from the learning dataset. The accuracy of the NN predictions . 


## Beginning: Initial ML model results

## Test 1: Removing Noisy Features 
The goal of optimization is to increment the smallest changes possible to the model until the model has the desired accuracy score. Rather than increase the amount of processing needed or risk overfitting right away, the stimulus is removing a low impact feature. In this case the "Organization" feature was removed.
</br>
</br>

## Results
![3](./Images/layer_accuracy.png)
</br>
</br>

## Test 2: Changing number of Hidden Layers
The model is reverted back to the initial test state, this is done by replacing the "Organization" feature removed in test 1. The new stimulus is the addition of another hidden layer, and adjusting each layer to have 16, 8, 4, and 2 units respectively.

## Results
![4](./Images/hiddenlayer.png)
</br>
</br>

## Test 3: Increasing Number of Epochs
The model is used as it exists after the previous test. The new stimulus is the addition of 25 epochs to the model.

## Results
![5](./Images/epochs.png)
</br>
</br>

## Test 4: Combo
The model is used as it exists after the previous test. The new stimulus is the addition of the "Name" column, the addition of a hidden layer, changing layer units to 64, 32, 16, and 8 respectively, and finally the addition of 25 epochs to the model (150 total).

## Results
![6](./Images/final.png)
</br>
</br>

## Summary
More testing is needed at the time of writing to determine a method by which the accuracy of the model will reliably reach over 75%. 
