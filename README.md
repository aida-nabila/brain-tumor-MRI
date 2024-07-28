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

## Setting Up Kaggle API
**Step 1: Generate Kaggle API Token**
1. Go to your Kaggle account settings: Account.
2. Scroll down to the "API" section and click on "Create New API Token". This will download a kaggle.json file containing your API credentials.

**Step 2: Set Up Kaggle API in Google Colab**
1. Upload the kaggle.json file to your Google Drive.
2. Mount your Google Drive in Google Colab and copy the kaggle.json file to the appropriate directory:

```
from google.colab import drive
drive.mount('/content/drive')

!mkdir -p ~/.kaggle
!cp /content/drive/My\ Drive/path_to_your_kaggle.json ~/.kaggle/kaggle.json
!chmod 600 ~/.kaggle/kaggle.json
```
Replace path_to_your_kaggle.json with the actual path to your kaggle.json file in Google Drive.

# Results
The models are evaluated based on the following metrics:

- Test Accuracy
- Mean Average Precision (mAP)
- Training Time
- Model Complexity (Number of Parameters)
