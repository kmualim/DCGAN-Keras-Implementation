# DCGAN Implementation

An inital implementation of a Deep Convolutional General Adversarial Network (DCGAN) initially on MNIST dataset available. 
The following repository has different files: 
1. DCGAN-Keras-Implementation-MNIST.ipynb 
2. download.py 
3. dcgan-mnist.py 

Things to note: 
After every 50 training iterations, a .png file will be saved locally within the colab notebook environment or on your disc depending on which you've used to run. 
Both the ipynb and python script can be used to run the model; ipynb notebook, however, have the before and after images as well as the plotted loss graphs. 

## Dependencies: 
* [Python 3.6](https://www.python.org/downloads/) 
* [Keras](https://keras.io/#installation) 
* [matplotlib](https://matplotlib.org/users/installing.html) (mainly for data visualization)
* [NumPy](https://docs.scipy.org/doc/numpy-1.13.0/user/install.html)

## Introduction: 
Applying Deep Convolutional Generative Adversarial Nets to generating MNIST images. 

![](https://github.com/kmualim/DCGAN-Keras-Implementation/blob/master/files/dcgan-image.png)
Image from [1]. 

## Data: 
The dataset consists of 60,000 **28x28** grayscale images of 10 digits, along with a test set of 10,000 images. 
In this implementation, we only utilized the training set.
To download: 
```
`from keras.datasets import mnist`
`(x_train, y_train), (x_test, y_test) = mnist.load_data()`
```
or alternatively: 
```
`$ python download.py` 
```
## Usage: 
To run the experiment with default parameters:
1. download the ipynb notebook 
2. run the ipynb notebook

or alternatively:
```
`$ python dcgan-mnist.py` 
```
Parameters can be changed in `dcgan-mnist.py`

Values are documented in the ipynb notebook for easy reference.

## References: 
1. https://medium.com/@jonathan_hui/gan-dcgan-deep-convolutional-generative-adversarial-networks-df855c438f



