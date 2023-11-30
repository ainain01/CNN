# DeepVisionNet_CNN
# Report:
# Approach:
# Data Preprocessing:
-Dataset split into training and validation sets.
-Appropriate data augmentation techniques applied for improved generalization.
# Model Architecture:
# Convolutional Layers:
-Layer 1: Convolutional layer with 28 filters, ReLU activation, batch normalization, max-pooling (2x2), and dropout (p=0.5).
-Layer 2: Convolutional layer with 44 filters, ReLU activation, batch normalization, max-pooling (2x2), and dropout (p=0.5).
-Layer 3: Convolutional layer with 76 filters, ReLU activation, batch normalization, max-pooling (2x2), and dropout (p=0.5).

# Fully Connected Layers:
-FC1: Linear layer with 512 neurons, ReLU activation, batch normalization, and dropout (p=0.5).
-FC2: Linear layer with the number of output classes.

# Output Layer:
-Softmax activation applied.

# Hyperparameters:
-Learning rate: 0.001
-Batch size: 32
-Dropout rate: 0.5
-Optimizer: Adam
-Loss function: CrossEntropyLoss
# Training:
-Model trained for 10 epochs.
-Training and validation accuracy monitored at each epoch.
# Results:
# Before Training:
-Convolutional layer outputs obtained for sample images.
-Final output tensor obtained through the softmax activation.

# After Training:
-Training started with low accuracy and high loss.
-Accuracy steadily increased with each epoch.
-After the 4th epoch, the model achieved 100% accuracy on both training and validation sets.
-Challenges and Solutions:

# Challenges:
-Initially, the model started with low accuracy.
-There might have been issues with model convergence.
# Solutions:
-Adjustments made to hyperparameters, including learning rate and dropout rate.
-Batch normalization and dropout layers added to enhance model generalization and mitigate overfitting.
# Conclusion:
-The model achieved 100% accuracy on both training and validation sets after 4 epochs.
-Hyperparameter tuning significantly improved model performance.
-Batch normalization and dropout played crucial roles in preventing overfitting.
