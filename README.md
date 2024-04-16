# Function Approximation using Neural Networks

- **Author:** Arshia Goshtasbi

- **GitHub:** [@Arshiagosh](https://github.com/Arshiagosh)
## Introduction

This Python code demonstrates how to approximate various functions using a multilayer perceptron (MLP) neural network. The code is divided into four sections, each focusing on a different function:

1. Simple Function: `f(x) = x^2`
2. Polynomial Function: `f(x) = x^3 - 2x^2 + 3x - 1`
3. Trigonometric Function: `f(x) = sin(2x) + cos(3x)`
4. Complex Function: A piecewise function with different expressions for different intervals of the input domain.

The code follows a common structure for each function, including steps for generating synthetic data, scaling the input data, defining the neural network architecture, compiling the model, training the model using cross-validation, inverse scaling for visualization, plotting the best fold prediction, and visualizing the training and validation loss for all folds.

The key steps in the code are as follows:

1. Generate training and test data for the given function.
2. Scale the input data using `MinMaxScaler` from `sklearn.preprocessing`.
3. Define a sequential neural network model using `keras.models.Sequential` and `keras.layers.Dense`.
4. Compile the model with a mean squared error loss function and the Adam optimizer.
5. Perform 5-fold cross-validation training using `sklearn.model_selection.KFold`.
6. Evaluate the model on the validation set for each fold and keep track of the best-performing fold.
7. Inverse scale the test input data for visualization purposes.
8. Plot the true function and the best fold prediction on the test data.
9. Visualize the training and validation loss curves for each fold.

The code utilizes various Python libraries such as NumPy, Matplotlib, Keras, and Scikit-learn for data generation, visualization, and model training/evaluation.

This code serves as a practical example of how to use neural networks for function approximation tasks and can be extended or modified to fit different use cases or functions.