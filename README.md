# Brain Tumor Classification: A Comparative Analysis of VGG16, ResNet50, Xception, and MobileNets Convolutional Neural Networks on MRI Images

<div align="center">
    <img width="400" src="/images/sanple_images_brain_tumor_dataset.png" alt="Material Bread logo"> 
    <p style="text-align: center;">Photo created by autor</p> 
</div>


## My Medium Articles on Brain Tumor Classification
- Brain Tumor Classification: Analysis of VGG16, ResNet50, Xception, and MobileNets Convolutional Neural Networks on MRI Images[Medium](https://medium.com/@t.mostafid/brain-tumor-classification-analysis-of-vgg16-resnet50-xception-and-mobilenets-convolutional-a7445638a233)

- Overview of VGG16, ResNet50, Xception and MobileNet Neural Networks [Medium](https://medium.com/@t.mostafid/overview-of-vgg16-xception-mobilenet-and-resnet50-neural-networks-c678e0c0ee85)

## Introduction:

This project employs **deep learning** to classify brain tumors in MRI scans, emphasizing a comparative analysis of  various **transfer learning** approaches.
Four distinct deep neural network models, namely **VGG16**, **MobileNet, Xception, and ResNet50 models**, we categorize brain tumors into four classes: No Tumor, Glioma, Meningioma, and Pituitary.
These models predict the presence of a brain tumor based on MRI scans, and their comparative analysis offers insights into their performance for brain tumor classification.

- Source of data [Brain Tumor](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri)

## Brain Tumor Classification Dataset
The dataset consists of 3264 MRI images. 926 are “gliomas”, 937 are “meningiomas”, 901 are “pituitary” tumors, and 500 are images representing cases without tumors. Figure 1 illustrates sample images from each class, showing significant inter- and intra-class diversity.

The dataset was randomly divided into 2870 training and 394 test sets for the experiments. Figure below illustrates the statistics of the training and test sets, showing a notable difference in the distribution of classes between them. This difference poses a challenge for CNN models to generalize from the trained model to the test set. In addition, both sets exhibit class imbalances, presenting an additional challenge to the models. For training, a validation set consisting of 15% of the training set was randomly sampled with a class distribution similar to the training set.


<div align="center">
    <img width="1000" src="/images/train_test_distribution.png" alt="Material Bread logo"> 
    <p style="text-align: center;">Photo created by autor</p> 
</div>

## Model Training
During the training phase, the specified models are trained on the training dataset and validated on the validation set. A consistent batch size of 64, the Adam optimizer, and the Categorical Cross Entropy loss function are used for all models. Due to variations in structure and parameter count, different learning rates are assigned to ensure effective training, and different numbers of epochs are implemented to prevent overfitting as the models converge.

<div align="center">
    <img width="1200" src="/images/vgg_accuracy_loss.png" alt="Material Bread logo"> 
    <p style="text-align: center;">Photo created by author</p> 
</div>

<div align="center">
    <img width="1200" src="/images/ResNet50_accuracy_loss.png" alt="Material Bread logo"> 
    <p style="text-align: center;">Photo created by author</p> 
</div>

<div align="center">
    <img width="1200" src="/images/Xception_accuracy_loss.png" alt="Material Bread logo"> 
    <p style="text-align: center;">Photo created by author</p> 
</div>

<div align="center">
    <img width="1000" src="/images/MobileNet_accuracy_loss.png" alt="Material Bread logo"> 
    <p style="text-align: center;">Photo created by author</p> 
</div>



## Model Evaluation:

The trained models are then tested on the test dataset. Considering the training and validation curves, the best epoch is selected when the loss is the smallest, the accuracy is the largest for the training, and just before the model starts overfitting when the validation curves start to diverge. Therefore, for VGG16 epoch 15, for ResNet50 epoch 46, for Xception epoch 20, and for MobileNet epoch 50 are considered for evaluation.

<div align="center">
    <img width="1000" src="/images/model comparison.png" alt="Material Bread logo"> 
    <p style="text-align: center;">Photo created by author</p> 
</div>


## Conclusion and Future work:
  - Satisfactory performance observed for VGG16, Xception, and MobileNet in the Brain Tumor Classification dataset.
  - Exception for ResNet50, which exhibited suboptimal performance.
  - Noteworthy success in classifying "meningioma" and "no-tumor" cases.


<div align="center">
    <img width="800" src="/images/Results.webp" alt="Material Bread logo"> 
    <p style="text-align: center;">Photo created by author</p> 
</div>


## Future Work Suggestions and Overall Research Direction
  - Explore dataset expansion and diversification to enhance model robustness.
  - Implement data augmentation techniques to address class imbalances.
  - Investigate the impact of hyperparameter tuning for improved model performance.
  - Explore alternative optimizers and loss functions to optimize the training process.
  - Address the challenges posed by misclassifications through further investigation.
  - Future studies should focus on refining the model's ability to handle diverse and imbalanced datasets.
  - Avenues for improvement include algorithmic enhancements and exploration of advanced optimization techniques.






