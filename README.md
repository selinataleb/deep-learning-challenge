# deep-learning-challenge

Overview: 

The purpose of this analysis is to create a machine learning model that predicts whether an organization funded by Alphabet Soup will be successful. Using a deep neural network, we preprocess the data, train an initial model, optimize the model for better performance, and evaluate its results. The target accuracy for the model is above 75%.

Results: 

The columns EIN and NAME were removed because they do not contribute to the prediction.
We encoded categorical variables such as APPLICATION_TYPE and CLASSIFICATION in order to transform them into numerical values.
We used StandardScaler for a better model performance. 
For our base model: First hidden layer had 80 neurons with a ReLU activation function.
Our second hidden layer had 30 neurons with a ReLU activation function.
And lastly, our output layer 1 neuron with a sigmoid activation function for binary classification. 
The model used the adam optimizer and binary_crossentropy as the loss function and was trained for 100 epochs with a validation split of 15%.

The training accuracy was: 73.81%
The validation accuracy was: 73.65%
The training loss: 53.21%
The validation loss was: 54.35%

For our optimization, we decided to increase the number of neurons in the first-hidden layer from 80 to 100 and the second later from 30 to 50. We then added a third hidden layer with 25 neurons to improve the model's ability to identify patterns. 
The training accuracy was: 73.86%
The validation accuracy was: 73.65%
The training loss: 52.86%
The validation loss was: 56.31%

Summary 

The baseline model acheives an accuracy of 72.69% and a loss of 56.50% while the optimized model gave us an accuracy of 72.88%, and a loss of 57.96%. 
Although our target accuracy of 75% was not achieved, the results are very close to 75%. 

I recommend adding more neurons to the hidden layers for the model to help capture more complex patterns, also adding additional hidden layers. We could possibly adjust the activation functions from ReLu to tanh 
