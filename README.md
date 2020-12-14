## Overview
The purpose of this project is to use machine learning and neural networks to create a binary classifier that is capable of predicting applicatants that will be succesful if funded by Alphabet Soup.

## Results

* Data Preprocessing
  * The variables IS_SUCCESFUL and STATUS are considered the targets for the model. 
  * The variable IS_SUCCESFUL are considered the feature for the model.
  * The variables that were not needed and should be removed for the model are EIN and NAME.

* Compiling, Training, and Evaluating the Model
  * For the AlphabetSoupCharity the number of hidden layers that was used was 2 because there were 2 variables that were considered targets for the model. The total number of neurons that wwas used was 110. This amount was selected because of the amount of columns in the application_df. Relu was selected as the activation for the model because the model is looking at positive nonlinear input data for classification or regression.
  * The model was unable to achieve the target model performance since the accuracy was 69.5%.
  ![picture]
  
  * When building the optimization model I tried to increase the bins by changing the type_count from 500 to 600 and the class_count from 800 to 900. Which caused a decrease in columns in the merged dataframe application_df. Next, I decreased the number of input features from 80 to 70 for the first layer. For the second layer I decreased it from 30 to 20. Also, I added in a 3rd hidden layer with 5 input features. Lastly I decreased the epochs from 100 to 90. By doing all this the accuracy actually decreased to 54.5%.
  ![picture]
  
## Summary
Overall I would say my optimziation didn't work and I would recommend switching to a Random Forest Deep Learning to see if the accuracy will increase. 
