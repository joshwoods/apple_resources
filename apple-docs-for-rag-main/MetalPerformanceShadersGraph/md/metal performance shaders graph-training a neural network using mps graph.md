

- Metal Performance Shaders Graph
-  Training a Neural Network using MPS Graph 

Sample Code

# Training a Neural Network using MPS Graph

Train a simple neural network digit classifier.

Download

iOS 14.0+iPadOS 14.0+Xcode 14.3+

## Overview

The sample code describes how to write a neural network using MPSGraph and how to train the network to recognize a digit in an image. The sample trains a network for 300 iterations on a batch size of 40 images. You’ll see how to set up training of weights and biases using data sources, including how to initialize and update weights. You’ll also see how to validate the network using a test dataset.

Note

This sample code project is associated with WWDC 2020 session 10677: Build customized ML models with the Metal Performance Shaders Graph.

You can use any dataset of your choice to train this model. The following dataset works well for this purpose:

MNIST Dataset

Please note that Apple does not own the copyright to this dataset nor makes any representations about the applicable terms of use for this dataset.

If you choose to use this dataset, the sample includes a script that downloads the dataset from that location and pass it as input to the model.

### Configure the Sample Code Project

This sample requires the following system and software configuration:

- macOS 11 or later

- iOS 14 or later

- Xcode 12 or later

