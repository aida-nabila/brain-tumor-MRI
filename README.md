# Brain Tumor MRI classification
This project involves training and evaluating three different Convolutional Neural Networks (CNNs) on a dataset of brain tumor MRI images. 
The goal is to classify the images into different categories based on the presence of tumors. The CNNs used in this project are ResNet50, DenseNet121, and MobileNetV3.

# Project Description
Brain tumors can be life-threatening, and early detection is crucial for effective treatment. This project aims to develop a reliable classification system for brain tumor 
MRI images using state-of-the-art deep learning models. Three different CNN architectures are employed:

- ResNet50
- DenseNet121
- MobileNetV3
  
Each model is trained on the same dataset, and their performance is compared based on accuracy, mean Average Precision (mAP), training time, and model complexity.

# Data Modelling
## Models
Three different CNNs are used for training the dataset. These networks are available within the Keras library and are trained for 50 epochs each.

### ResNet50

Number of Parameters: Approximately 23.5 million <br>
Description: A deep CNN with residual connections that help in training very deep networks by mitigating the vanishing gradient problem.

### DenseNet121

Number of Parameters: Approximately 8 million <br>
Description: A CNN that uses dense connections, ensuring efficient gradient flow and feature reuse. It balances complexity and performance effectively.

### MobileNetV3

Number of Parameters: Approximately 5.4 million <br>
Description: A lightweight CNN designed for mobile and edge devices, focusing on efficiency and speed with fewer parameters.

# Metrics
Two metrics are used to observe the performance of the models:

- Accuracy
- Mean Average Precision (mAP)
  
Additionally, the training time for each model is recorded.

# Results
The models are evaluated based on the following metrics:

- Test Accuracy
- Mean Average Precision (mAP)
- Training Time
- Model Complexity (Number of Parameters)

# Performance Summary

| Model | Test Accuracy | mAP | Training Time (seconds) | Parameters |
|---|---|---|---|---|
| MobileNetV3 | 0.67 | 0.53 | 12424.56 | 5.4 million |
| DenseNet121 | 0.96 | 0.98 | 39842.43 | 8 million |
| ResNet50 | 0.71 | 0.65 | 17574.55 | 23.5 million |

Based on the results, DenseNet121 achieved the highest test accuracy and mAP, making it the best-performing model despite its longer 
training time. MobileNetV3 is the most efficient in terms of training time and parameter count, suitable for resource-constrained environments.
