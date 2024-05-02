# Custom Neural Network for Coffee Roasting Classification

This code snippet demonstrates an alternative approach to implement a neural network model for coffee roasting classification using custom-defined functions instead of TensorFlow's Keras API. Here's a breakdown of the key components and steps involved:

## Data Preprocessing
- The coffee roasting dataset is loaded and visualized using `plt_roast`, displaying features such as temperature and duration of roasting alongside corresponding labels indicating the quality of coffee roasting.

![Plot-Coffee-Roasting-Data](https://github.com/UMMY87/Custom-Neural-Network-for-Coffee-Roasting-Classification/assets/117314436/f3df1459-997a-48c2-98a3-ad8150213cc0)

- The features are normalized using TensorFlow's `Normalization` layer to standardize the data and improve model performance.

## Custom Neural Network Implementation
- Custom functions are defined to construct the neural network model:
  - `my_dense`: Computes the dense layer operation, taking input data, weight matrix, and bias vector as inputs and producing the output activations.
  - `my_sequential`: Combines multiple dense layers sequentially to form the complete neural network architecture.
  - `my_predict`: Generates predictions by applying the custom-defined neural network model to input data.

## Prediction and Decision Making
- Predictions are made on test data (`X_tst`) using the `my_predict` function with weights and biases initialized earlier.
- Decision making is performed by applying a threshold of 0.5 to the predictions to classify examples into positive or negative categories.

## Visualization
- The neural network's decision-making process and predictions are visualized using the `plt_network` function, which illustrates the model's decision boundaries on the coffee roasting dataset.
![Plot-of-network-probability- -decision](https://github.com/UMMY87/Custom-Neural-Network-for-Coffee-Roasting-Classification/assets/117314436/1e83be76-d13d-4dfe-bd19-d601aa892125)

Overall, this code provides an alternative approach to building and evaluating a neural network model for coffee roasting classification, showcasing the flexibility of implementing custom neural network architectures using NumPy and Python.
