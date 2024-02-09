# Autoencoder
## Overview
This Python code implements a multilayer perceptron autoencoder for image compression and reconstruction. The autoencoder is designed to compress input images into a latent space and then reconstruct them.
## Features
- Input layer accommodating RGB images (3 channels).
- Adjustable number of hidden neurons and dimensions.
- Training with backpropagation and momentum for weight updates.
- Early stopping based on reconstruction error threshold.
## Architecture
The autoencoder follows a three-layer structure:

1. **Input Layer:**
   - Neurons: Input neurons are configured to match the dimensions of the image.

2. **Hidden Layer (Latent Space - Encoder):**
   - Neurons: Adjustable number of hidden neurons multiplied by the specified dimensions.

3. **Output Layer (Reconstruction - Decoder):**
   - Neurons: Same configuration as the input layer to reconstruct the image.

## Functions
- `forward_propagation`: Performs forward propagation through the autoencoder.
- `back_propagation`: Performs backpropagation to update weights based on reconstruction error of the output image.
- `sigmoid_function`: Computes the sigmoid function and its derivative (as needed).
- `train`: Trains the autoencoder for a specified number of epochs.
- `test`: Reconstructs an image using the trained autoencoder.
## Dependencies
- NumPy
- Matplotlib
- Pillow (PIL)
## Example
![Reconstructed Image](https://github.com/21zasker/Autoencoder/blob/main/Screenshots/Results_image.png)
## Note
Example input images are provided on the **Resources** folder.
