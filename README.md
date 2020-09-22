# Semantic Segmentation
## What is Semantic Segmentation?

Semantic segmentation refers to the process of linking each pixel in an image to a class label. It can also be referred to as **image classification** for pixels in an image. Its primary applications include autonomous vehicles, human-computer interaction, robotics and photo-editing tools. It is very useful for 
delf-driving cars in which contextual information of the environment is required at each and every step while traversing the route.

![alt text](https://miro.medium.com/max/1000/1*wbaUQkYzRhvmd7IjKJjjCg.gif)

## Aim of this project
What we aim to do in this project is to perform semantic segmentation on CAMVID dataset and evaluate the deep learning model by using some metrics.

## Deep Learning architecture
For this project, I am going to use unet architecture, which was developed by Olaf Ronneberger et al. for Bio Medical Image Segmentation. The architecture of this model is similar to that of an autoencoder. The encoding path consists of a series of convolutions, also known as the down-sampling path. The decoding path consists of upconvolutions (transposed convolutions are used in this case). It's also called the up-sampling path. The architecture of unet is fully convolutional, wherein we are using the Cross Entropy Loss.

![alt text](https://miro.medium.com/max/1600/1*OkUrpDD6I0FpugA_bbYBJQ.png)

## Specific details of the dataset used
The Cambridge-driving Labeled Video Database (CamVid) is the first collection of videos with object class semantic labels, complete with metadata. The database provides ground truth labels that associate each pixel with one of 32 semantic classes.

## Deep Learning Framework used
I=We have used PyTorch as the deep learning framework for this task.

## Steps involved


1.   Data-preprocessing
2.   Data-loading (using custom dataloaders)
3.   Developing the deep learning architecture
4.   Training the model
5.   Evaluating the model:
     1.   Pixel Accuracy
     2.   Intersection over Union
6.   Testing for a particular sample image
