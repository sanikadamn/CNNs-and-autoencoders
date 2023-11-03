# CNNs and Autoencoders

## Datasets used
- `MNIST` and `mnist-with-awgn.mat` (a noisy version of MNIST)

## CNNs
- The first part of `CNNs_autoencoders.ipynb` contains the code for a CNN trained on the MNIST dataset.
- I have used 2 convolutional layers, dropout, and a fully connected layer.
- The ReLU activation function is used for the convolutional layers.
- The loss function used is CrossEntropyLoss, which includes softmax activation.
- I have added code to visualize the feature maps after each layer.

## Autoencoders
- Autoencoders and decoders have been used to denoise the noisy dataset.
- 1. For denoising the noisy MNIST, I have first introduced noise to the normal MNIST dataset and found the optimal parameters for reconstructing the image.
- 2. Used this model to encode and decode images in the noisy dataset.
- 3. Used the previously trained model to evaluate the now denoised datset.