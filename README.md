# Hyper-Parameter-Tuning
### This project demonstrate Hyperparameter Tuning with Keras Tuner to tune a Convolutional Neural Network for Fashion MNIST dataset. Also you will see the concept of transfer learning and fine-tuning.
## Prerequisites
- Python 2.x

## Installing Dependencies
<b>Note: You can skip this step, if you already installed the packages that mentions below. Dependencies are listed in the requirements.txt file</b> 
## Necessary Libraires or packages are:-
- TensorFlow
- Keras
- Numpy
- Hyperas, Hyperopt
- Matplotlib

You will need an IPython notebook to try this on your project or to follow along.
<b> If you install pip, then you can install the dependencies by running pip3 install -<name of dependencies></b>

## Concepts
### Pre-Process Data
 - We Load the data from the keras.datasets
 - We are only provided with a train and test set as we also need a validation set we use scikit-learn’s train-test split to split train data obtained into 80% train and 20% validation
 - Changing the shape of the train validate and test data from 28x28 format to a list of 784 values.
- Normalizing our input so that the input values range from 0 to 1 rather than 0 to 255, Standardization can also be done.
- Also since we have used categorical cross-entropy we need to convert our output to one-hot encoded form this can be done easily as follows.

## Transfer learning
For this part I have used Mobilenet network from keras applications as pretrained model and I have implemented my object and non-object images in this pretrained model.
Here, I have used a Mobilenet model which was pre-trained on the ImageNet dataset by fine-tuning it on the Fashion-MNIST dataset. The Mobilenet model is a convolutional block (several layers in each block) deep learning network built on the ImageNet database.

<b> After fine-tuning, the test accuracy of the model is almost 78% which is greater than the tesst accuracy from part 3. Hence, we can conclude that the transfer learning and fine tune is the best model to implement in our dataset, even if we have small number of data, we could get pretty good accuracy.</b>

