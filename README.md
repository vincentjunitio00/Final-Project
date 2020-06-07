# Beans

Bangkit Academy Final Project

## Dataset Description

Dataset from : https://github.com/AI-Lab-Makerere/ibean/

This dataset consists of leaf images taken in the field in different districts in Uganda by the Makerere AI lab in collaboration with the National Crops Resources Research Institute (NaCRRI), the national body in charge of research in agriculture in Uganda.

| Class             | Total Examples|
| ----------------- | ------------- |
| Healthy class     | 428           |
| Angular Leaf Spot | 432           |
| CBean Rust        | 436           |
| Total             | 1,296         |

## Dataset Sample

<img src="https://i.ibb.co/ZL6mkpy/beans-0-1-0.png" width="500" height="400">

## Goal 

The data is leaf images representing 3 classes: the healthy class of images, and two disease classes including Angular Leaf Spot and Bean Rust diseases. The model should be able to distinguish between these 3 classes with high accuracy. The end goal is to build a robust, model that can be deployed on a mobile device and used in the field by a farmer.

## Base CNN Model

The CNN base model architecture consists of 3 pair of Conv-Pool layers and 1 hidden layer at fully connected layer without dropout layer(s). There is no image augmentation applied on the training images.

<img src="https://i.ibb.co/qjWW2xM/Screen-Shot-2020-05-25-at-23-11-21.png" width="350" height="300">

## Improved CNN Model

The improved CNN Model architecture consists of the same 3 pairs of Conv-Pool layers and 1 hidden layer at fully connected layer, with 2 dropout layers after the 1st Conv-pool layer and after the 3rd Conv-Pool layer. Image augmentation is applied on the training images: rotation, width shift, height shift, shear, zoom, and horizontal flip.

<img src="https://i.ibb.co/bWpkyYM/Screen-Shot-2020-05-25-at-23-24-08.png" width="350" height="300">

Image augmentation visualization

<img src="https://i.ibb.co/5r4Qnhg/imgaug.png" width="600" height="100">

## Evaluation Comparison

Base CNN model's accuracy and loss

<img src="https://i.ibb.co/5MhR7b3/Screen-Shot-2020-05-25-at-23-40-26-copy.png" width="450" height="300">

Improved CNN model's accuracy and loss

<img src="https://i.ibb.co/kgGr43N/Screen-Shot-2020-05-25-at-23-40-26.png" width="450" height="300">






