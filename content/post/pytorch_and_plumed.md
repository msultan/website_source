+++
date = "2017-08-14"
draft = false
image = ""
tags = ["pytorch", "plumed","enhanced sampling","Neural networks"]
title = "Collective variables as computational graphs"
math = false
summary = """
 Using PyTorch to enhance molecular simulations and using Plumed to classify images
"""
+++
I spent the weekend desiging a project to show how complex PyTorch computational graphs can
be turned into collective variables inside Plumed. This was done in two parts.

[PyTorchMetadynamics.ipynb]((https://github.com/msultan/tf_metadynamics/blob/master/PyTorchMetadynamics.ipynb))

This Jupyter notebook encodes Metadynamics into PyTorch using a custom loss function depenedent on the history.
The forces then become the negative of the derivatives which are automatically obtained via back propagation.
This was performed on the Muller potential.

[PlumedImagesNeuralNetwork.ipynb](https://github.com/msultan/tf_metadynamics/blob/master/PlumedImagesNeuralNetwork.ipynb)

This Jupyter Notebook transfers a 3-layer Image Net PyTorch Classifier into Plumed, encodes the
images as molecular trajectories, and use Plumed to predict the un-normalized image scores.
The plumed input file image_plumed.dat has the actual plumed neural network script.


All the code + details are available on my [github](https://github.com/msultan/tf_metadynamics).