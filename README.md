# Deep-Learning-Challenge

## Overview 

The purpose of this challenge and this analysis is that the nonprofit foundation Alphabet Soup wants a tool to help them select applications for funding with the best chance of success in thier ventures. In the challenge it is the use of machine learning and neural networks to create a binary classifer that will be able to predict wheather applicants will be successful if funded by Alphabet Soup. 

## Process

To start the process I read the csv file provided which contained 34,000 organizations that have received funding from Alphabet Soup over the years. The target of this analysis is whether the organization will be successful or not if Alphabet Soup gives them funding. This means we are really paying attention to the IS_SUCCESSFUL column. We want the model to achieve a targer predictive accuracy higher than 75%. To begin with we droped the EIN and NAMe columns. We then found the amount of unique values for each column and for the columns that had more than 10 unique values we determined the number of data points for each unique value. We then bined the data to make it easier to work with. Then we got dummie variables for the categorical variables. Then we split the preprocessed data into arrays and split the data. Then we are ready to comppile, train, and evaluate the model.

## 1st Test

 - The Application_type cutoff is 500
 - The Classification cutoff is 900
 - The first hidden layer is 10
 - The second hidden layer is 5
 - There are 100 epochs
 - The loss is 55.60%
 - The accuracy is 73.71%

## 2nd Test 

  - The Application_type cutoff is 500
  - The Classification cutoff is 900
  - The first hidden layer is 15
  - The second hidden layer is 10
  - There are 100 epochs
  - The loss is 55.36%
  - The accuracy is 73.74%

## 3rd Test

  - The Application_type cutoff is 500
  - The Classification cutoff is 900
  - The first hidden layer is 50
  - The second hidden layer is 20
  - There are 100 epochs
  - The loss is 56.20%
  - The accuracy is 74.06%

## 4th Test

  - The Application_type cutoff is 500
  - The Classification cutoff is 900
  - The first hidden layer is 80
  - The second hidden layer is 40
  - There are 100 epochs
  - The loss is 58.60%
  - The accuracy is 73.48%

## Summary 

In all four of my attempts I was not able to reach the target predictive accuracy of 75% or higher. The closest I came to reaching the target was in the 3rd test where I reached an accuracy of 74.06%. I was about 1% off from the target. Throughout this whole challenge I kept it with only two hidden layers and just decided to play around with how many were in each hidden layer. I also used the activations of "tanh" and "relu" throughout all of the challenge as well. If I were to go back and do it again I might change up which activations I used in the challenge and maybe I would decide to add another hidden layer. I would also maybe change the cutoff values for the application_type and the classificaiton. This might cause the model to better predict which organizations would be successful if Alphabet Soup gave them money. While I did not hit the target accuracy I did come close and I would say that the model in the 3rd attempt is the best out of the four attempts at predicting which organizations would be successful if Alphabet Soup were to give them money.

