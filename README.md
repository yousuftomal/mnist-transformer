# MNIST Digit Classification with Transformer

This project implements a Transformer-based model for classifying handwritten digits from the MNIST dataset. The model uses a custom Transformer architecture adapted for image classification tasks.

## Features

- Custom Transformer architecture for image classification
- MNIST dataset preprocessing and loading
- Model training and evaluation
- TensorFlow and Keras implementation

## Requirements

To run this project, you need Python 3.7+ and the following libraries:

- TensorFlow 2.x
- NumPy

For a complete list of dependencies, see `requirements.txt`.

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yousuftomal/mnist-transformer.git
   cd mnist-transformer
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Ensure you have the MNIST dataset (`mnist.npz`) in the `/kaggle/input/mnist-dataset/` directory.

2. Run the main script:
   ```
   python mnist_transformer.py
   ```

The script will load the MNIST data, preprocess it, create and train the Transformer model, and finally evaluate its performance on the test set.

## Model Architecture

The model consists of:
- A custom TokenAndPositionEmbedding layer
- A TransformerBlock with multi-head self-attention and feed-forward network
- Global Average Pooling
- Dense layers for final classification

## Results

After training for 10 epochs, the model achieves 96% accuracy on the test set.


## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgements

- The MNIST dataset providers
- TensorFlow and Keras teams