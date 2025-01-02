Overview of the Code:
![Screenshot 2025-01-02 210131](https://github.com/user-attachments/assets/c400fb58-d83b-404f-a33b-c7aa75c8a700)

Project Name: Image Classification Using Deep Learning

Objective:
To build and evaluate a Convolutional Neural Network (CNN) for classifying images from the CIFAR-10 dataset into one of 10 classes, such as airplanes, automobiles, birds, etc.

Key Activities:

Data Preprocessing:

Dataset Loading: The CIFAR-10 dataset is loaded using TensorFlow's keras.datasets.
Normalization: The pixel values of images are scaled to the range [0, 1] for better training efficiency.
One-Hot Encoding: Labels are converted to one-hot encoding for multi-class classification.
Model Definition:

A CNN model is built using TensorFlow's Sequential API.
Convolutional Layers: Two convolutional layers with ReLU activation extract spatial features from the images.
Pooling Layers: Max pooling reduces the spatial dimensions, preserving important features.
Dense Layers: Fully connected layers handle feature classification, with a final softmax layer outputting probabilities for each class.
Training and Validation:

The model is compiled with:
Optimizer: Adam optimizer for adaptive learning.
Loss Function: Categorical cross-entropy for multi-class classification.
Metric: Accuracy to monitor model performance.
The model is trained for 10 epochs with a batch size of 64, and validation is performed on the test dataset.
Evaluation and Visualization:

Evaluation: The model's accuracy on the test dataset is calculated and displayed.
Training History Visualization: Plots are generated to visualize training and validation accuracy and loss across epochs.
Prediction Visualization: A few test images are displayed along with their predicted class labels.
Model Saving:

The trained model is saved as cifar10_model.h5 for future use.
Technologies Used:

Libraries: TensorFlow (for model building and training), Matplotlib (for visualizations), NumPy (for data manipulation).
