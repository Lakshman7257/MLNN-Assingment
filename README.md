Understanding Autoencoders: How Neural Networks Learn to Reconstruct Images
Overview
This repository contains a machine learning tutorial on autoencoders using the Fashion-MNIST dataset. The tutorial explains how a neural network can learn to reconstruct images by compressing them into a smaller bottleneck representation and then rebuilding them through a decoder.
The main teaching focus is:
How does the bottleneck control what the autoencoder remembers?
Unlike a classification model, the autoencoder does not predict labels such as shirt, shoe or bag. Instead, it learns to reproduce its own input. The input image is also the target output.
Learning Objectives
By following this tutorial, the reader will learn how to:
Understand the basic structure of an autoencoder.
Explain the role of the encoder, bottleneck and decoder.
Prepare Fashion-MNIST images for reconstruction learning.
Train a dense autoencoder using TensorFlow and Keras.
Interpret reconstruction loss during training.
Compare original and reconstructed images.
Analyse how different bottleneck sizes affect reconstruction quality.
Tutorial Concept
An autoencoder has three main parts:
1.Encoder
Compresses the input image into a smaller representation.
2.Bottleneck
Stores the compressed latent code. This limits how much information can pass through the model.
3.Decoder
Reconstructs the image from the bottleneck representation.
The tutorial compares bottleneck sizes of 8, 32 and 64 to show how stronger compression affects image reconstruction.
Dataset
The tutorial uses the Fashion-MNIST dataset. It contains 28 x 28 grayscale images of clothing items such as shirts, shoes, dresses, bags and sandals.
Although Fashion-MNIST includes class labels, the labels are not used to train the autoencoder. The model learns from the image itself.
Repository Structure
autoencoder-reconstruction-tutorial/
│
├── README.md
├── LICENSE
├── lakshman_naik_code.ipynb
├── lakshman_naik_banavathu_24155315.pdf
│
└── figures/
    ├── figure_1_sample_images.png
    ├── figure_2_autoencoder_structure.png
    ├── figure_3_reconstruction_loss.png
    ├── figure_4_original_vs_reconstructed.png
    ├── figure_5_bottleneck_size_comparison.png
    └── figure_6_reconstruction_error_by_bottleneck.png


How to Run the Notebook
1.Clone or download this repository.
2.Install the required packages:
1.Open the notebook:
jupyter notebook lakshman_naik_code.ipynb
1.Run the notebook cells from top to bottom.
The notebook downloads Fashion-MNIST automatically through TensorFlow/Keras, so no manual dataset download is needed.
Requirements
The tutorial was written using Python and the following main libraries:
tensorflow
numpy
matplotlib
jupyter
A  requirements.txt file is:
tensorflow
numpy
matplotlib
jupyter
