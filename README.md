# Image_Classifier_Deep_Learning
# Deep Learning - PyTorch
Developing a Neural Network for an image classifier to train on the CIFAR-10 dataset

## Introduction 
Building an image classifier and object detection system using PyTorch.

The aim is to build a image classification neural network using PyTorch, and train it to classify the CIFAR-10 dataset with decent (>70%) accuracy

## Walkthrough of Project Steps

The following are the main steps of this project

1. Explore and prepare the data for training and testing.
2. **Design and build the neural network.**
3. Train the neural network on the training set.
4. Evaluate your network's performance on the test set.

**Step 2** is the most important step of this project. Inorder to build a neural network, instead of building the convolution layers ourselves, 
we will utilize transfer learning of **Resnet-50** deep convolution network. 

The last _fully-connected_ layer of the Resnet-50 is substituted with our own fully connected layer with 10 outputs (for the CIFAR-10 dataset)

## Notes
The project **requires a GPU** run and will not work well (be extremely slow) if run on a local CPU.

The project was run on the GPU enabled workspaces within the Udacity classroom.  

Due to the limited access to a GPU enabled workspace, the following improvements, instead of being implemented, are marked as _future_ improvements

## Future improvements
* Instead of freezing the Resnet-50 convolution backbone, unfreeze the whole network and let it train on the CIFAR-10 dataset. This might improve the accuracy of the network 
and bring it close to 90%
* Instead of using transfer learning of Resnet-50, try building own Convolution Neural Network (CNN). The accuracy of the self made CNN will be lower than Resnet-50, 
but it will be good practice

