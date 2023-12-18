# Brain Tumor Classification: A Comparative Analysis of VGG16, ResNet50, Xception, and MobileNets Convolutional Neural Networks on MRI Images


## Brain_Tumor_Classification

<div align="center">
    <img width="400" src="/images/sanple_images_brain_tumor_dataset.png" alt="Material Bread logo"> 
    <p style="text-align: center;">Photo created by autor</p> 
</div>



## My Medium Articles on Brain Tumor Classification
- Overview of VGG16, ResNet50, Xception and MobileNet Neural Networks [Medium](https://medium.com/@t.mostafid/overview-of-vgg16-xception-mobilenet-and-resnet50-neural-networks-c678e0c0ee85)
  
- Brain Tumor Classification: A Comparative Analysis of Convolutional Neural Network Architecture on MRI Images [Medium](https://medium.com/p/a7445638a233/edit)

## Introduction:

This project employs **deep learning** to classify brain tumors in MRI scans, emphasizing a comparative analysis of  various **transfer learning** approaches.
Four distinct deep neural network models, namely **VGG16**, **MobileNet, Xception, and ResNet50 models**, we categorize brain tumors into four classes: No Tumor, Glioma, Meningioma, and Pituitary.
These models predict the presence of a brain tumor based on MRI scans, and their comparative analysis offers insights into their performance for brain tumor classification.

- Source of data [Brain Tumor](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri)

## What is brain tumor?

A brain tumor refers to an accumulation of abnormal cells in the brain, presenting a significant health concern due to its aggressive nature. Magnetic Resonance Imaging (MRI) stands out as the most effective technique for detecting brain tumors.

## Data Augmentation and Rescaling

Data augmentation involves applying various transformations to the existing dataset to create additional training examples. These transformations, such as rotation, flipping, or zooming, help enhance the model's ability to generalize and perform well on unseen data. Data augmentation is particularly useful improving the neural network's ability to handle translation invariance.

Apply rescaling to all three datasets (train, validation, and test) for comparability. However, limit data augmentation techniques to the training dataset only, excluding the test and validation sets. This ensures that the model is evaluated on its ability to make predictions on unseen, unaltered data during the testing and validation phases.

## What is transfer learning?

Transfer learning accelerate deep CNN model training by reusing weights from pre-trained models on a large dataset, such as MobileNet with ImageNet weights. This approach is valuable for smaller datasets, providing an effective shortcut to model training. It involves adapting a pre-trained model to related tasks with limited labeled data, enhancing learning efficiency across various applications like image classification, object detection, etc.

## 

  
## Conclusion and Future work:
  - Satisfactory performance observed for VGG16, Xception, and MobileNet in the Brain Tumor Classification dataset.
  - Exception for ResNet50, which exhibited suboptimal performance.
  - Noteworthy success in classifying "meningioma" and "no-tumor" cases.


## Future Work Suggestions and Overall Research Direction
  - Explore dataset expansion and diversification to enhance model robustness.
  - Implement data augmentation techniques to address class imbalances.
  - Investigate the impact of hyperparameter tuning for improved model performance.
  - Explore alternative optimizers and loss functions to optimize the training process.
  - Address the challenges posed by misclassifications through further investigation.
  - Future studies should focus on refining the model's ability to handle diverse and imbalanced datasets.
  - Avenues for improvement include algorithmic enhancements and exploration of advanced optimization techniques.






