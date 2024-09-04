# Water Segmentation Using U-Net

This project focuses on segmenting water bodies from multi-channel images using a U-Net model. The dataset used in this project consists of TIFF images with 12 channels and corresponding binary mask labels in PNG format. The U-Net model was built from scratch without utilizing any transfer learning, and it produced impressive results.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training Process](#training-process)
- [Results](#results)
- [Usage](#usage)


## Project Overview

This project aims to accurately segment water bodies from satellite images using a deep learning model. The U-Net architecture was chosen due to its effectiveness in image segmentation tasks, particularly when working with multi-channel inputs.

## Dataset

- **Images:** The dataset contains images in TIFF format, each with 12 channels. These images represent various spectral bands, providing detailed information for accurate segmentation.
- **Labels:** The corresponding labels are binary masks in PNG format, indicating the presence or absence of water in each pixel of the images.

## Model Architecture

The U-Net model was designed from scratch to handle the unique characteristics of the multi-channel input data. The architecture consists of an encoder-decoder structure with skip connections, enabling the model to capture both spatial and contextual information.

- The full structure of the U-Net model is provided in the `U-net model.py` file.

## Training Process

The model was trained on the multi-channel TIFF images, with the binary masks serving as labels. Key details of the training process include:

- **Input Dimensions:** (128, 128, 12)
- **Loss Function:** Custome Dice loss function
- **Optimizer:** Adam
- **Data Augmentation:** Horizontal flip was applied to increase the robustness of the model.

## Results

The U-Net model achieved remarkable accuracy in segmenting water bodies, demonstrating its effectiveness in this task. The detailed results, including metrics such as accuracy, precision, and recall
## Usage

To use the code in this repository:

1. Clone the repository:
   ```bash
   git clone https://github.com/username/water-segmentation-unet.git
