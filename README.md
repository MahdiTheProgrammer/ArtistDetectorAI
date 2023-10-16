# Artistic Similarity Model: Unleashing AI to Identify the Echoes of Renowned Artists in Your Paintings! 
### Welcome to  Artistic Similarity Model – This project focuses on leveraging the power of neural networks to determine which artist's style your artwork most closely resembles. 


<img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Tsunami_by_hokusai_19th_century.jpg"/>

## Table of Contents
#### Introduction
#### Android Application
#### Dependencies
#### Useful Functions
#### Dataset
#### Data Preprocessing
#### Model Architecture
#### Training
#### Results

## Introduction
Art is a reflection of human expression, and every artist possesses a unique style that defines their creations. By utilizing machine learning techniques, I have trained a model that focuses on leveraging the power of neural networks to determine which artist's style your artwork most closely resembles.<br>
In the Quora link provided above, it's evident that this project has the potential to greatly benefit artists. <br>
<a href="https://www.quora.com/How-do-I-find-an-artist-who-has-an-art-style-similar-to-mine">Click here </a>

## Android Application
Now you can experience the power of AI with your phone! I have developed an Android application based on this model.
<br><br><br>
<img src="https://play-lh.googleusercontent.com/P5Z0HKuTYjcj6F1jvSgxYHgAmEqHdyfG6Ts0lDfcKVDGIyfLLs43tw41GQMM4q48TQ=w240-h480-rw" style="border: 2px ; border-radius: 50px;   display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;"/>


## Dependencies
Make sure you have the following dependencies installed:

```
import torch
from tqdm.auto import tqdm
import numpy as np
import random
import os
from PIL import Image
from torch.utils.data import Dataset, DataLoader
import matplotlib.pyplot as plt
from torchvision.transforms import transforms
from timeit import default_timer as timer
from torch import nn
import torch.quantization
from torch.quantization import QuantStub, DeQuantStub, quantize_dynamic
from collections import OrderedDict
import torch.optim as optim 
```

## Useful Functions
I have included several utility functions for data analysis, plotting, accuracy calculation, and more. These functions are contributed by Daniel Bourke and are helpful for visualizing and interpreting the project's progress.

## Dataset
I created a dataset comprising grayscale images of artworks from 10 renowned artists, including Andy Warhol, Claude Monet, Edvard Munch, Henri Matisse, Leonardo da Vinci, Michelangelo, Pablo Picasso, Rembrandt, Salvador Dali, and Vincent van Gogh.

## Data Preprocessing
The dataset is loaded, preprocessed, and transformed into appropriate formats for training and evaluation. I also provide a function to display sample images from the dataset.

## Model Architecture
I tried different convolutional neural network (CNN) architectures to extract features from the paintings effectively. The final chosen architecture is a CNN with two convolutional layers followed by two max-pooling layers, and two fully connected layers for classification.

## Training
The model is trained using the training dataset, with the Adam optimizer and cross-entropy loss function. I perform 30 epochs of training and monitor both training and testing loss and accuracy.

## Results
The results of the training process are displayed and interpreted. I showcase the progression of training loss and accuracy over epochs.

## Status
The first official version is available in 
```
project.ipynb
```  
file. <br><br>
9/16/2023 <br>
I am currently working on the second version which can get acc of 80%. The code will be available in 
```
project_v2.ipynb
```
file. <br><br>
9/17/2023 <br>
Code in 
```
project_v2.ipynb
```
directory works with acc of 80%. Comments will be added soon.


