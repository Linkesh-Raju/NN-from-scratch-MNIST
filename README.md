# NN-from-scratch-MNIST

A 2-layer neural network built with only NumPy. No TensorFlow. No PyTorch.
It classifies handwritten digits from the MNIST dataset.

## Results
Best run (lr 0.50, 500 iterations)
Train accuracy: 90.5%
Test accuracy: 88.0%

## Architecture
Input: 784 pixels (28x28)
Hidden layer: 10 neurons, ReLU
Output layer: 10 neurons, softmax

## What I implemented
Forward propagation
Backpropagation
Gradient descent
One-hot encoding
Accuracy evaluation

## My changes
Tested two learning rates, 500 iterations each.
lr 0.10: train 79.7%, test 74.9%
lr 0.50: train 90.5%, test 88.0%

lr 0.10 is undertrained at 500 iterations. It learns too slowly.
lr 0.50 converges faster. In one run, train accuracy swung between iterations.
The train/test gap is small (2.5 points), so little overfitting.

## Credit
Based on Samson Zhang's "Neural Network from Scratch" tutorial.
I followed the video, then ran the learning rate experiments above.

## How to run
1. Download the MNIST CSV from Kaggle (Digit Recognizer).
2. Open the notebook in Jupyter or Kaggle.
3. Run all cells.

## Requirements
Python 3, NumPy, pandas, Matplotlib
