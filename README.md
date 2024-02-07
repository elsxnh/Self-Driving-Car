# Self-Driving-Car-UNet

📁 Created by: Elsa Nurul Hidayah, 2023

This repository is created to fulfill the bootcamp Computer Vision project requirement from Indonesia AI.

🔬 This project is aimed at addressing the challenges of traffic congestion in large cities through the use of image segmentation. By leveraging the Cityscapes dataset, which contains images captured from a car's perspective within specific urban environments, the project focuses on developing a robust image segmentation algorithm using the UNet architecture with ResNet101 as the encoder.

## Problem Statement

Traffic congestion is a major issue in urban areas, leading to increased travel times, pollution, and accidents. The goal of TrafficNet is to utilize advanced computer vision techniques, particularly image segmentation, to analyze and understand roads and obstacles in real-time. The ultimate objective is to contribute to the development of self-driving cars powered by artificial intelligence, capable of efficiently navigating through congested city streets.

![Example](https://www.intelligenttransport.com/wp-content/uploads/self-driving-1.jpg)

## Dataset

The project employs the Cityscapes dataset, which includes a diverse set of images taken from within cars, providing a realistic view of urban environments. The dataset is annotated with pixel-level segmentation masks for various classes, such as sky, building, road, car, pedestrian, and more. This rich dataset allows the model to learn and generalize effectively for urban scene understanding. Link: https://www.cityscapes-dataset.com/

![Dataset](https://www.cityscapes-dataset.com/wordpress/wp-content/uploads/2015/07/exampleFeaturedImage-270x250.png)

## Model Architecture

TrafficNet utilizes a UNet architecture with ResNet101 as the encoder. The key specifications of the model include:

- Encoder: ResNet101
- Encoder Weights: ImageNet pre-trained
- Classes: ['sky', 'building', 'pole', 'road', 'pavement', 'tree', 'signsymbol', 'fence', 'car', 'pedestrian', 'bicyclist', 'unlabeled']
- Activation: Softmax2D

The choice of ResNet101 as the encoder and Softmax2D activation aims to capture intricate details in urban scenes and produce pixel-wise segmentation predictions.

## Results 

## Implementation Details

The project is implemented in PyTorch and makes use of the segmentation_models_pytorch library. The model is trained on a GPU if available; otherwise, it falls back to CPU. To run this project on your local machine using Google Colab connected to Google Drive, follow these systematic steps:

### Prerequisites

Before you begin, make sure you have the following prerequisites:

1. Google Colab account
2. Access to Google Drive
3. Dependencies (in the section below)

### Procedure

1. Open Google Colab and navigate to the notebook located in the project's directory.

2. Mount Google Drive within the Colab notebook by executing the following cell:

    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```
3. Clone the repository to your google colab (recommended):

    ```bash
   git clone https://github.com/elsxnh/Person-Tracking-YOLOv8.git](https://github.com/elsxnh/Self-Driving-Car.git)https://github.com/elsxnh/Self-Driving-Car.git
    ```
