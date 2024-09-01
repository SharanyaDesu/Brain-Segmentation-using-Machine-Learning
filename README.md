# Brain-Segmentation-using-Machine-Learning

Brain Segmentation in Training Images 

![Training Images segmentation](https://github.com/user-attachments/assets/180f7d29-4660-4844-a6b7-029ff218c444)


Brain segmentation in Testing Images

![Testing Image Segmentation](https://github.com/user-attachments/assets/b279ac4e-c795-4436-832f-0744ef9384da)


# Project Overview
This project focuses on segmenting brain tumors from MRI images using deep learning techniques. The primary model utilized is the U-Net architecture, which is well-suited for medical imaging tasks. The project involves detailed preprocessing steps, custom data generation, and the implementation of a U-Net model to accurately segment tumor regions in MRI scans.


# Methodology

# U-Net Model
Encoder: Extracts high-level features from MRI images using a series of convolutional and pooling layers.

Decoder: Upsamples the features and merges them with corresponding encoder features to produce a precise segmentation mask.

Activation & Regularization: The model uses ReLU activation functions and dropout layers to introduce non-linearity and prevent overfitting.


# Custom Data Generator

Memory Efficiency: Handles large MRI images by loading and preprocessing data in batches.

On-the-fly Preprocessing: Performs real-time preprocessing steps such as MRI slice resizing, normalization, and segmentation mask processing.

Customization: Allows flexibility in defining preprocessing steps tailored to the dataset and model requirements.

# Preprocessing Steps
Defined data paths for MRI scans and segmentation masks.

Resized MRI slices to a consistent dimension (e.g., 128×128px) for uniform input to the U-Net model.

Normalized MRI intensity values to ensure consistent data scaling.

# Segmentation Process

The U-Net model was trained on preprocessed MRI data, capturing tumor regions with high accuracy.

The segmentation mask was evaluated using metrics like Accuracy, Mean IoU, and Dice Coefficient, ensuring robust performance.

# Results

The model achieved high training accuracy with:

Model 1: Learning rate of 0.0001, Training Accuracy: 98.63%

Model 2: Learning rate of 0.00001, Training Accuracy: 98.33%

Sample segmentation results on test images demonstrated the model's ability to identify tumor regions effectively.


# Conclusion
The project showcases the power of CNN-based deep learning models, particularly U-Net, in medical image segmentation tasks. Despite using a relatively small dataset, the model achieved impressive results. Further improvements could be made by increasing the dataset size and refining preprocessing techniques to focus solely on brain regions, excluding background noise.
