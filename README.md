# Neural_Network_Charity_Analysis

## Overview of the Project 

Alphabet Soup is a non-profit foundation that raises and donates funds to philanthropic causes. However, not every recipient uses the donated money in the way it was intended to be spent.
The purpose of this analysis was to create a binary classifier that is capable of predicting whether applications will be successful if funded by Alphabet Soup.
The binary classifier was created using the features available in the dataset, which contains over 34 000 organizations that have been funded by Alphabet Soup over the years 

## Results

### Data Preprocessing 

1) What variable(s) are considered the target(s) for your model?

The target variable in this model is the "IS_SUCCESFUL" column in the dataset.

2) What variable(s) are considered to be the features for your model?

The variables that were features in this model: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS" and "ASK_AMT".

3) What variable(s) are neither targets nor features, and should be removed from the input data?

The "NAME" and "EIN" variables were neither features nor targets.

### Compiling, Training, and Evaluating the Model

1) How many neurons, layers, and activation functions did you select for your neural network model, and why?

<img width="749" alt="hiddenlayers" src="https://user-images.githubusercontent.com/97644424/179836228-c9609ce6-c413-48ed-9187-05bd5d33614c.PNG">

I selected three hidden layers with different levels of neurons on each level. The first level had 80 neurons, the second had 30 neurons and the third layer had 15 neurons. I used the reluv and tanh activation function. I made these choices to improve the accuracy of the model.

2) Were you able to achieve the target model performance?

Even after several attempts to modify the model, I was unable to achieve the target model performance of 75%. The accuracy performance level I achieved was 0.7319.

3) What steps did you take to try and increase model performance?

The steps I took to increase model performance was to add a third hidden layer and change the activation function. I also attempted to try the random forest model as well. 

<img width="750" alt="Activation Functions" src="https://user-images.githubusercontent.com/97644424/179836466-857fcd5a-14bb-4caf-b78d-660131e38e73.PNG">

<img width="740" alt="randomforest" src="https://user-images.githubusercontent.com/97644424/179836526-ae4559e7-a6a0-42a9-a2d8-2ad8bc3df3b9.PNG">

## Summary

<img width="453" alt="accuracyoriginal" src="https://user-images.githubusercontent.com/97644424/179835938-32011106-7155-46eb-a795-8e5095e91f94.PNG">

The original model (prior to optimization) had an accuracy of 0.7277.

<img width="454" alt="accuracyoptimization" src="https://user-images.githubusercontent.com/97644424/179836116-b0e4d467-e0c3-4b31-9ddb-c3aaa579ae29.PNG">

After optimization, which included adding another hidden layer and using the tanh activation function, the model had an accuracy of 0.7319. Using a different model like the random forest model could increase the accuracy of this learning model as random forest because it has high accuracy and high interpretability. 