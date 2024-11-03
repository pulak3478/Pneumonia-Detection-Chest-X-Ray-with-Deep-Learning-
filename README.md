# Pneumonia-Detection-Chest-X-Ray-with-Deep-Learning-

## Overview
This project presents a deep learning-based approach to automate pneumonia detection using chest X-ray (CXR) images. Traditionally, CXR interpretation requires expertise, leading to potential delays and variability in diagnosis. This project leverages convolutional neural networks (CNNs) to streamline the detection process, reducing reliance on manual expertise and aiming to provide a reliable, efficient diagnostic aid.

## Dataset
The model is trained and validated on the Chest X-Ray Images (Pneumonia) dataset containing 5,850 labeled images: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

- **Classes**: Normal (healthy) and Pneumonia (infected).
- **Data Source**: Available on Kaggle, providing a large set of labeled CXR images.

## Preprocessing
To enhance image quality and feature extraction, Contrast Limited Adaptive Histogram Equalization (CLAHE) is applied to each image, improving the visibility of features crucial for accurate diagnosis.

## Model Architecture
Two CNN architectures are used in this project:

- **InceptionV3**: Known for its high accuracy in image classification tasks.
- **ResNet50V2**: A powerful deep learning model with residual connections to handle complex image data.
Both models are fine-tuned using transfer learning to optimize their performance for pneumonia detection.

## Performance
Initial results show the following:
ResNet50V2: Training accuracy of 98% and validation accuracy of 92.71%, demonstrating strong potential as a reliable diagnostic tool.

## Project Structure
- **data**: Contains datasets used for training and testing.
- **preprocessing**: Includes scripts for image preprocessing (CLAHE application).
- **models**: Contains the InceptionV3 and ResNet50V2 model architectures.
- **training**: Scripts to train and evaluate models.
- **results**: Performance metrics and evaluation reports.
