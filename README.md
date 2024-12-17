# MNIST Classification with PyTorch

This project implements a neural network for classifying handwritten digits using the MNIST dataset.<br>
The model is built and trained using PyTorch, with CrossEntropyLoss as the loss function.<br>
The training and testing accuracies are plotted for performance evaluation.

## Dataset
The MNIST dataset is automatically downloaded using the `torchvision.datasets` module.

- Training Data: 60,000 handwritten digit images
- Test Data: 10,000 handwritten digit images

## Model Architecture
The model is a fully connected feedforward neural network with ReLU activation functions:

- Input Layer: 28x28 (flattened to 784)

- Hidden Layers:
  - Layer 1: 1024 neurons
  - Layer 2: 1024 neurons

- Output Layer: 10 neurons (one for each digit 0–9)
The final layer outputs logits, which are directly passed to the CrossEntropyLoss function.

## Training
The model is trained using Stochastic Gradient Descent(SGD) with a learning rate of 0.001 for 100 epochs.

- Loss Function: CrossEntropyLoss
- Optimizer: SGD with Momentum (optional: momentum=0.9 for faster convergence)

## Results
![image](https://github.com/user-attachments/assets/cca0868c-ab49-4e95-9513-8118e9af85bd)

