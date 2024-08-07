# Visualizing Decision Boundaries for an AND Gate Neural Network Model


## Overview

This project demonstrates how to visualize the decision boundaries of a neural network trained to model an AND gate. By using Python, TensorFlow, and Keras, we can build a simple yet effective neural network and visualize how it learns to separate different classes through decision boundaries.

## Features

- **Neural Network Architecture:** A simple feedforward neural network using TensorFlow and Keras.
- **Data Visualization:** Decision boundaries are visualized using Matplotlib to provide insights into the model's learning process.
- **Interactive Experience:** Users can experiment with different hyperparameters and observe changes in decision boundaries.

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [How it Works](#how-it-works)


## Installation

### Prerequisites

Ensure you have the following installed on your machine:

- Python 3.x
- [TensorFlow](https://www.tensorflow.org/install)
- [Keras](https://keras.io/getting_started/)
- [NumPy](https://numpy.org/install/)
- [Matplotlib](https://matplotlib.org/stable/users/installing.html)

### Clone the Repository

```bash
git clone https://github.com/your-username/and-gate-neural-network.git
cd and-gate-neural-network
```

### Install Dependencies

Use `pip` to install the required Python packages:

```bash
pip install -r requirements.txt
```

Create a `requirements.txt` file with the following content if you haven't already:

```plaintext
tensorflow
keras
numpy
matplotlib
```

## Usage

Run the script to train the neural network and visualize the decision boundaries:

```bash
python visualize_and_gate.py
```

### Adjusting Hyperparameters

You can modify the hyperparameters in the `visualize_and_gate.py` file to see how they affect the model:

```python
# Example hyperparameters
learning_rate = 0.01
epochs = 100
hidden_layer_neurons = 4
```

## How it Works

### 1. Data Preparation

The dataset used consists of all possible input combinations for an AND gate:

| Input 1 | Input 2 | Output |
|---------|---------|--------|
| 0       | 0       | 0      |
| 0       | 1       | 0      |
| 1       | 0       | 0      |
| 1       | 1       | 1      |

### 2. Model Architecture

The neural network consists of an input layer, a hidden layer, and an output layer:

- **Input Layer:** 2 neurons (for the two input features)
- **Hidden Layer:** 4 neurons (adjustable)
- **Output Layer:** 1 neuron (for binary classification)

### 3. Training

The model is trained using backpropagation and the Adam optimizer. The learning rate and the number of epochs are configurable.

### 4. Visualization

The decision boundary is visualized using Matplotlib to show how the neural network distinguishes between classes.

