# Deep Learning Case Study: Model Building and Network Comparison

## Brain_Tumor_Classification

<div align="center">
    <img width="400" src="/images/brain-outline-drawing-12.png" alt="Material Bread logo"> 
</div>

## Introduction:

This project employs **deep learning** to classify brain tumors in MRI scans, emphasizing a comparative analysis of  various **transfer learning** approaches.
Three distinct deep neural network models, namely **MobileNet, Xception, and ResNet50 models**, we categorize brain tumors into four classes: No Tumor, Glioma, Meningioma, and Pituitary.
These models predict the presence of a brain tumor based on MRI scans, and their comparative analysis offers insights into their performance for brain tumor classification.

- Source of data [Brain Tumor](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri)

## What is brain tumor?

A brain tumor refers to an accumulation of abnormal cells in the brain, presenting a significant health concern due to its aggressive nature. Magnetic Resonance Imaging (MRI) stands out as the most effective technique for detecting brain tumors.

## Motivation and Goals:

Provide valuable support to neurosurgeons and radiologists by offering a cost-effective and non-invasive means of brain tumor detection. The key objectives of this project are:

1. Develop a Neural Network model aimed at the classification of whether a patient has a brain tumor or not.

2. Comapre different transfer learning and 3 deep neural network models, i.e. MobileNet,Xception,ReseNet50 in order to classify the Brain MRI Images to 4 different independent classes.

3. Implement a segmentation process on MRI images to accurately separate tumor regions from normal brain tissues.

## What is transfer learning?

Transfer learning accelerate deep CNN model training by reusing weights from pre-trained models on a large dataset, such as MobileNet with ImageNet weights. This approach is valuable for smaller datasets, providing an effective shortcut to model training. It involves adapting a pre-trained model to related tasks with limited labeled data, enhancing learning efficiency across various applications like image classification, object detection, etc.


## Compare 3 deep neural network models:


1. **MobileNet:**
   - MobileNet is a lightweight neural network architecture designed for mobile and embedded vision applications. It is trained on the ImageNet dataset, and its efficient design makes it suitable for real-time image classification on resource-constrained devices.

2. **Xception:**
   - Xception is an extension of the Inception architecture, and it has also been trained on the ImageNet dataset. Xception focuses on improving the efficiency of learning hierarchical features from data. It has shown strong performance in image classification tasks.

3. **ResNet50:**
   - ResNet50 is part of the ResNet (Residual Network) architecture, specifically ResNet-50, which contains 50 layers. It is a deep convolutional neural network that excels in feature extraction and image classification. ResNet50 has been trained on the ImageNet dataset and has achieved state-of-the-art performance.




