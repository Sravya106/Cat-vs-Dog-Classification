# Cat-vs-Dog-Classification
Deep learning model to classify dog and cat images

## Overview

This repository contains code for a Cat-Dog classification project using machine learning. The goal is to train a model to distinguish between images of cats and dogs. The dataset used for this project consists of a collection of labeled cat and dog images.

## Getting Started
Data was taken from imported Kaggle. 

## Dataset

The dataset includes the following:

- **Images**: A collection of cat and dog images.
- **Labels**: Binary labels indicating whether the image contains a cat (1) or a dog (0).
- **val_data**: a small amount of data is seperated from training data for validation.


### Data Preparation
Data preparation includes resizing and rescaling the images. Accationally a data agumentation is applied. For this model data resizing and data rescaling layers 
are added to the model itself.

### Model Building and Training
The technique used to build this model was **transfer learning** which enables us to use a pre-trained model such as GoogLeNet, VGGNet etc. 

## Model Architecture

The neural network used for this visualization is based on the following architecture:

- **Resizing**
- **Rescaling**
- **VggNet base model**
- **Convolutional layer with 16 3x3 filters**
- **MaxPooling**
- **Flatten**
- **Dense layer**
- **Dropout layer**
- **output layer**

### Model Training
**optimizer**: Adam
**metrics**: accuracy
**callbacks**: Learning rate scheduler, Early Stopping

**Model Accuracy**: 80%

