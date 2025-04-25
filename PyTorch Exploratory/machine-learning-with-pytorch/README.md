# Machine Learning with PyTorch

This project demonstrates how to build, train, evaluate, and save a simple neural network for handwritten digit recognition using PyTorch and the MNIST dataset.

## Overview

The notebook covers the following steps:
- **Setup:**  
  Installs and imports required libraries including PyTorch and TorchVision.
- **Data Loading:**  
  Downloads the MNIST dataset and prepares DataLoaders for training and testing.
- **Model Definition:**  
  Implements a feedforward neural network with two hidden layers and ReLU activations.
- **Training:**  
  Trains the model using cross-entropy loss and the Adam optimizer.
- **Evaluation:**  
  Tests the model on unseen data and reports accuracy and average loss.
- **Saving and Loading:**  
  Saves the trained model parameters and demonstrates how to reload them for inference.

## Key Features

- **MNIST Dataset:**  
  Uses a standard dataset of 28x28 grayscale images of handwritten digits (0-9).
- **Neural Network:**  
  Simple architecture with input, hidden, and output layers.
- **Training Loop:**  
  Includes a custom training function with periodic loss reporting.
- **Testing Loop:**  
  Evaluates model accuracy and loss on the test set.
- **Model Persistence:**  
  Shows how to save and reload model weights for future predictions.

## Usage

1. **Install dependencies:**
    ```bash
    pip install torch torchvision
    ```

2. **Run the notebook:**  
   Open `Machine_Learning_with_PyTorch.ipynb` in Jupyter or VS Code and execute the cells step by step.

## File Structure

- `Machine_Learning_with_PyTorch.ipynb` — Main notebook with code, explanations, and results.
- `README.md` — Project overview and instructions.

## References

- [PyTorch Documentation](https://pytorch.org/docs/stable/index.html)
- [TorchVision Documentation](https://pytorch.org/vision/stable/index.html)
- [MNIST Dataset](http://yann.lecun.com/exdb/mnist/)

---

**Author:** Adapted from IBM Developer tutorial  
**License:** For educational use