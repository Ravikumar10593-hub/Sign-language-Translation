# Sign-language-Translation
It's a working project of Sign language Translation which is also called as American Sign Language (ASL) translation,It is the primary sign language used by the deaf and people with hearing impairment in the USA and Canada.

# First start with importing all the imp module required

import warnings
warnings.filterwarnings('ignore')
import os
import numpy as np
import pandas as pd
import tensorflow as tf
import matplotlib.pyplot as plt
from collections import Counter

# read all train data
data = pd.read_csv("D:/MLT/image mnist/sign_mnist_train/sign_mnist_train.csv")
print('Dataframe Shape:', data.shape)

# follow the screenhot from number 40 to 59

# to show the output
image, pred = get_prediction(x_test[5].reshape(1, 784)) # 5 mean 5th no of data image from data set
plt.imshow(image,cmap = 'binary') # binary to change the colour
plt.title(pred) # name of the symbol
plt.show() # show the scaling
