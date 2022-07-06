# object-detection

# Project Description
Object detection in low-illumination environments is very challenging. Due to insufficient reflected light under low-illumination, the image captured contains a lot of dark areas and noise.

We use Image Data Generator to apply image preprocessing like histogram equalization, performing scaling and feed the images in batches to our model for
training (to avoid memory issues while training). We will first train our own CNN model without applying any image processing to establish a baseline performance.
Then we will train an autoencoder on the training dataset. Then we will use the encoder of the autoencoder and feed its output to a CNN model and train the CNN
model. We will freeze the encoder layer while training the CNN model. The encoder here acts as a feature extractor that also performs dimensionality reduction
on the dataset. The idea of using this architecture is taken from this research paper [link](mdpi.com/1424-8220/21/22/7731). It has shown to improve accuracy of CNN models on various datasets over various CNN architectures. We hypothesize that we will also receive similar results.
