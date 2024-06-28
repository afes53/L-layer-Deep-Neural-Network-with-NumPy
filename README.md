# L-layer Deep Neural Network with NumPy
This project demonstrates the implementation of a deep neural network from scratch using NumPy. The network is designed to classify images based on their pixel values.

# Overview
## 1. Import Libraries and Load Data
The project starts by importing the necessary libraries, namely NumPy and Pandas. The dataset, which contains images represented as rows with pixel values in columns, is loaded from a CSV file. To facilitate processing, the dataset is transposed so that each column represents an image, and each row contains the pixel values.

## 2. Preprocess Data
The data is converted into a NumPy array and shuffled to ensure randomness. The dataset is then split into features (pixel values) and labels. The feature values are normalized to fall within a specific range.

## 3. Split Data into Training and Test Sets
The dataset is divided into training and test sets. Typically, 80% of the data is used for training, and 20% is used for testing. This helps in evaluating the model's performance on unseen data.

## 4. Initialize Network Parameters
The network architecture is defined by specifying the number of units in each layer. The weights and biases for each layer are initialized. Weights are initialized randomly with small values to break symmetry, while biases are initialized to zero.

## 5. Define Helper Functions
Several helper functions are defined to facilitate various operations within the neural network:

- Activation Functions: Functions like ReLU, Sigmoid, and Softmax are defined to introduce non-linearity in the network.
- Loss Functions: Functions to compute the loss for multiclass and binary classification are defined. These functions measure how well the network's predictions match the actual labels.
- Forward Propagation: This function computes the activations of each layer by performing matrix multiplications and applying the activation functions.
- Back Propagation: This function calculates the gradients of the loss with respect to the weights and biases using the chain rule. These gradients are essential for updating the network's parameters during training.

## 6. Parameter Update
The calculated gradients are used to update the network's weights and biases, minimizing the loss and improving the model's performance over time.

## 7. Utility Functions
Additional utility functions are provided to:

- Calculate the accuracy of predictions.
- Convert labels to one-hot encoding.
- Make predictions based on the trained model.
- Test the model on the test dataset.

## 8. Train the Model
The training function integrates all the above components. It iteratively performs forward and backward propagation, updates the parameters, and prints the training and test accuracy at specified intervals.

## 9. Evaluate the Model
After training, the model's performance is evaluated on the test dataset. The final trained model can make predictions on new data, and the accuracy of these predictions can be visualized and assessed.

##Conclusion
This project provides a comprehensive implementation of a deep neural network using NumPy, offering insights into the underlying mechanics of neural networks and their training process. It serves as an educational tool for understanding and building neural networks from the ground up.
