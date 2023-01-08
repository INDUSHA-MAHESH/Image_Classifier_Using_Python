# Image Classification Model Using Python

The model is built from scratch from collecting data, processing data, and constructing image dataset and training a model to classify the dataset

## Steps Involved

1. Data Collection
2. Data Augmentation
3. Data Transformation
4. Dataset Construction
5. Model Training and Testing

## 1. Data Collection

This project focuses on classifing 3 persons from eachother,  
I have chosen :  
- J K Rowling 
- Indra Nooyi 
- Michael Malarkey

and collected 10 images of each person.

## 2. Data Augmentation

Eventhough Construction of model with the collected 30 images is possible it is highly inefficient and produces a model with inadequate learning, hence we follow a approch of data augmentation.
In data augmentation a single image is used to create multiple images by shredding, zoominn in and out, changing aspect ratio etc,.
Hence increasing the dataset strength and number of training instances for the model

The augmented data is presented in the current repository, if you want to augument your own data and to know on how to do this process head to,  

https://github.com/INDUSHA-MAHESH/Data_Augmentation_Using_Keras

**After Data Augmentation each person had _312-380 images_**, a decent dataset indeed.  
  
  
![image](https://user-images.githubusercontent.com/71513343/211207854-a32a5687-90c1-488a-8b15-57e9bce5d1d1.png)


## 3. Data Transformation

The augmented data is put through a series of steps,

- Image Array Construction
- Grayscale Conversion
- Image Resize
- Image Array Flattening

## 4. Dataset Construction

With the flattened array for each image it becomes an instance of a dataset, convert them to a dataframe and add label
with the same procedure followed for each person concatenate the dataframe to one dataset.

## 5. Model Training and Testing

For now, I choose SVM to train the model.There are multiple models that would work for the data, but only one would be the best.
Inorder to choose it all the feasible models must be chosen and tested.

*Thank you for reading!*

