+++
date = "2017-08-14"
draft = false
image = ""
tags = ["pytorch", "plumed","enhanced sampling","Neural networks", "auto encoders"]
title = "Collective variables as computational graphs -- Part II"
math = false
summary = """
 Using Autoencoders to enhance molecular simulations via Metadynamics.
"""
+++
[Plumed](plumed.github.io) is a powerful library used for running enhanced sampling simulations. It implements a
very robust Collective variable module.

An autoencoder neural network is an unsupervised learning algorithm that tries to learn a latent space for its input.
This is done by setting the output to the input. Thus the network tries to learn an identity function.We can now use
this information, and restrict the middle layers of the encoding network to a singular value to
learn the most salient features of the data. More importantly, we can use enhance sampling techniques such as
metadynamics on this hidden layer to more efficiently sample alanine dipeptide.

[PlumedPyTorchAutoEncoderCV.ipynb](https://github.com/msultan/tf_metadynamics/blob/master/PlumedPyTorchAutoEncoderCV.ipynb)

The Jupyter Notebook transfers a 3-layer Enocder Neural network Plumed, for enhanced sampling via Metadynamics. The
resulting simulations are about 72x faster than regular MD alone.

All the code + details are available on my [github](https://github.com/msultan/tf_metadynamics).