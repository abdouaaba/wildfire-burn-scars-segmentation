# Wildfire Burn Scars Segmentation
This repository contains a Jupyter Notebook that shows how to augment a small dataset of 66 satellite images with corresponding burn scar masks, split the data into training and validation sets, and train a SegNet model to segment the burn scars of a wildfire in satellite images.

## Dataset
The dataset used in this project consists of 66 satellite images with corresponding burn scar masks. The images were obtained from a source that provides annotated images of wildfires.

## Augmentation
Since the dataset is relatively small, data augmentation techniques were used to increase the number of images. The augmentation techniques used include rotation, flipping, zooming, and shifting.

## Splitting
The dataset was split into a training set (70% of the images), a validation set (15% of the images) and a test set (15% of the images) using a random seed to ensure reproducibility.

## Model
The model used in this project is based on the SegNet architecture, which is an encoder-decoder architecture that uses convolutional and pooling layers in the encoder to extract features from the input image and upsampling and deconvolution layers in the decoder to recover the original image resolution. The model was trained using the augmented dataset and the Adam optimizer with a learning rate of 0.0001.

## Notebook
The Jupyter Notebook in this repository shows step-by-step how the dataset was augmented, split, and how the SegNet model was trained. The notebook also includes visualization of the training and validation loss, and examples of the burn scar segmentation on validation images.