# object-detection

# Project Description
Object detection in low-illumination environments is very challenging. Due to insufficient reflected light under low-illumination, the image captured contains a lot of dark areas and noise.

Dataset link: https://github.com/cs-chan/Exclusively-Dark-Image-Dataset

To enhance object detection capability of CNN image processing techniques like histogram equalization is applied. Then an autoencoder is trained on the training dataset. It will act as a feature extractor. Autoencoders is an unsupervised dimensionality reduction technique, which can filter out noise and redundant information and create robust and stable feature representations from image data. This convolutional autoencoder is utilised for compressing and filtering out noise and redundant information from initial high dimensionality input images and then this compressed output is fed into a convolutional neural network. 

This approach is adopted from this research paper: https://www.mdpi.com/1424-8220/21/22/7731


