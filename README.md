# Neural-Networks
Building Simple ANN from Stratch
This project shows how to build a simple neural network from scratch that can use chemical features of wine to guess how good it will be. The Wine Quality dataset from the UCI Machine Learning Repository was used for this project.

Set of data
The Wine Quality dataset was used. You can get it here. There are 1599 samples of red wine in the dataset. Eleven of the features reflect different chemical properties, and the target variable (a score between 0 and 10) shows how good the wine is.

Specifics
The dataset has the following features:

Level of acidity
Acidity in the air
Lemon juice
Sugar left over
Chlorides
No cost sulfur dioxide
All of the sulfur dioxide
Density
pH
The sulfates
Liquor
This is the goal variable:

Score from 0 to 10 for quality
Modeling and building
The following is how the neural network is built:

Eleven neurons make up the input layer—one for each trait.
Ten neurons in the hidden layer are activated by tanh.
Output layer: The number of neurons is equal to the number of unique classes in the goal variable, and they are activated with softmax.
Put into action Specifics
Getting data and doing preliminary work: The data is loaded, the target variable is turned into one-hot vectors, and StandardScaler is used to standardize the features.

Setting Up the Parameters: For each layer, the weights and biases are set up.

Message Sending Forward:

The data goes through the hidden layer when tanh is turned on.
To get the final results, the output from the hidden layer is sent to the output layer and softmax activation is used.
With backward propagation,

Backpropagation is used to figure out the gradients of the loss with respect to the weights and biases.
Gradient descent is used to change the weights and biases.
Training the Model: The model is trained for a set amount of time at a set rate of learning.

Prediction and Evaluation: The training model is used to guess what will happen with the test set, and its accuracy is measured.
