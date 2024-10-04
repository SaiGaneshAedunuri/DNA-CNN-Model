This project implements a Convolutional Neural Network (CNN) in PyTorch for classifying DNA sequences into distinct categories. The model leverages one-hot encoding to convert nucleotide sequences (A, T, C, G) into numerical inputs for the neural network, enabling effective sequence processing. The goal is to classify DNA sequences into predefined categories by leveraging deep learning techniques.

•	Model Architecture: A CNN model with multiple 1D convolutional layers, followed by fully connected layers, designed to capture patterns in DNA sequences. The model uses ReLU activations, max-pooling, and dropout regularization to improve performance.
•	Custom Dataset Loader: A custom PyTorch Dataset class was built to load DNA sequences from a text file. The DNA sequences are converted into one-hot encoded representations for input into the CNN.
•	Training and Testing Pipeline: The model is trained using the Adam optimizer with CrossEntropy loss. The training loop updates the model weights, while the testing loop evaluates accuracy and loss on unseen data.
•	GPU Acceleration: The project leverages CUDA for training the model on a GPU, significantly speeding up the training process for large DNA datasets.

Project Structure:
•	Model Definition: A Net class defines the CNN layers and forward pass.
•	Data Preprocessing: A function to one-hot encode DNA sequences, preparing them for input into the CNN.
•	Training Loop: The training process involves iterating through batches of data, computing loss, and backpropagating the gradients to update the model weights.
•	Testing Loop: The test loop evaluates model performance on a separate test set.

This project demonstrates the use of deep learning techniques for bioinformatics applications, specifically in the classification of DNA sequences.
