# Image-Classification-System-using-CIFAR10-Dataset

![alt text](/Photos/cifar10.PNG)

### Table of contents
* [Introduction](#introduction)
* [Problem Statement](#problem-statement)
* [Data Source](#data-source)
* [Technologies](#technologies)
* [Type of Data](#type-of-data)
* [Data Pre-processing](#data-pre-processing)
* [Algorithms Implemented](#algorithms-implemented)
* [Steps Involved](#steps-involved)
* [Evaluation Metrics](#evaluation-metrics)
* [Results and Conclusion](#results-and-conclusion)

### Introduction
In this project, we are going to design various neural networks by implementing their forward and backward passes. Given CIFAR-10 object detection dataset, we are going to implement four different neural networks. Softmax is the simplest without any hidden layer, which is essentially equivalent to a vanilla multiclass classification. TwoLayerNN has only one fully-connected hidden layer, which is often called Multi Layer Perceptron (MLP). ConvNet consists of convolutional hidden layers that alternate convolution, ReLU, and max- pooling operations. MyModel will be your customized model that must achieve the best performance on CIFAR-10 among these four models.

### Problem Statement
* Implement 4 different neural networks i.e. Softmax, TwoLayerNN, ConvNet and my own model(MyModel) on CIFAR10 after and obtain the best performance on your own customized      MyModel.

### Data Source
* The Dataset was obtained from the website: https://www.cs.toronto.edu/~kriz/cifar.html
  They were collected by Alex Krizhevsky, Vinod Nair, and Geoffrey Hinton.

### Technologies
* Python 3.6.7
* PyTorch 1.3

### Type of Data
* The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.
* Train : 50000
* Test  : 10000

### Data Pre-processing
* Normalizing of images

### Algorithms Implemented
* SoftMax
* TwoLayerNN
* ConvNet(CNN)
* Own Model including RESNET

### Steps Involved

* Import all the required libraries
* Downloading, Loading and Normalising CIFAR-10 using torch.utils.data.DataLoader and torchvision.transforms
* Display Random Batch of 4 Training Images using trainloader
* Defining the Convolutional Neural Network :  Input > Conv (ReLU) > MaxPool > Conv (ReLU) > MaxPool > FC (ReLU) > FC (ReLU) > FC (SoftMax) > 10 outputs
* Defining the Loss Function and Optimizer
* Train the Network
* Predicting the Category for all Test Images

### Evaluation Metrics  
Accuracy

![alt text](/Photos/acc.PNG)

### Results and Conclusion
After implementing 4 different neural networks i.e. Softmax, TwoLayerNN, ConvNet and my own model(MyModel) on CIFAR10, obtained the best performance on MyModel i.e. 92% accuracy

![alt text](/Photos/logv.PNG)
