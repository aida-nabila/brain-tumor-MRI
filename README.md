# Brain Tumor MRI classification
This project involves training and evaluating three different Convolutional Neural Networks (CNNs) on a dataset of brain tumor MRI images. 
The goal is to classify the images into different categories based on the presence of tumors. The CNNs used in this project are ResNet50, DenseNet121, and MobileNetV3.

# Project Description
Brain tumors can be life-threatening, and early detection is crucial for effective treatment. This project aims to develop a reliable classification system for brain tumor 
MRI images using state-of-the-art deep learning models. Three different CNN architectures are employed. These networks are available within the Keras library and are trained for 50 epochs each:

- ResNet50
- DenseNet121
- MobileNetV3
  
Each model is trained on the same dataset, and their performance is compared based on accuracy, mean Average Precision (mAP), training time, and model complexity.

# Dataset

The dataset consists of up to 20,000 brain tumor MRI images, categorized into three tumor classes (Glioma, Meningioma, and Pituitary) and one normal class.
You can find the dataset on Kaggle using the following link:
[Brain Tumors Dataset on Kaggle](https://www.kaggle.com/datasets/mohammadhossein77/brain-tumors-dataset)

# Getting Started
## Prerequisites

**Operating System**: Google Colab (platform-independent)

**Python Version**: Python 3.x

**Python Libraries**:
- `os`
- `shutil`
- `zipfile`
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `tensorflow`
- `keras`
- `sklearn`

# Results
The models are evaluated based on the following metrics:

- Test Accuracy
- Mean Average Precision (mAP)
- Training Time
- Model Complexity (Number of Parameters)
