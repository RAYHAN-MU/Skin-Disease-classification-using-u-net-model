
# Skin Disease Detection Using CNN based u-net model

## Project Overview 
🧠 Skin Disease Classification Using Modified U-Net Architecture
This repository contains the implementation of a skin disease image classification system developed as part of an undergraduate thesis.
The proposed approach utilizes a modified U-Net architecture adapted for image-level classification, as the dataset does not contain segmentation masks.

### Model Architecture
The proposed model is inspired by the U-Net architecture but modified for classification purposes.
Key Architectural Components
Encoder Path (U-Net Encoder)
Consists of multiple Double Convolution blocks
Each block includes:
3×3 Convolution
ReLU activation
3×3 Convolution
ReLU activation
2×2 Max Pooling

### Bottleneck Layer
Captures the most compressed and abstract feature representation
Expands feature depth for better discrimination
Converts feature maps into a fixed-length feature vector
Reduces the number of parameters
Helps prevent overfitting
Fully Connected Layer
Maps extracted features to final skin disease classes
🚫 Decoder path is removed, as segmentation is not performed.

### Training Details
Input image size: 224 × 224
Optimizer: Adam
Learning Rate: 1e-4
Batch Size: 8
Epochs:60

## Tools & Technologies
- Python
- NumPy, Pandas, Matplotlib
- PyTorch
- Google Colab

## Dataset
📂 Dataset Description  

## Skin disease image dataset
## Image-level class labels only 3000 images 
## No segmentation masks available
## Dataset split into:
## Training set
## Validation set
## Test set
Google Drive Link : https://drive.google.com/file/d/1HRnqVXgiUEvzHAzQ48_nZsuRyLaLc8f6/view?usp=drive_link

## Methodology
- Data preprocessing and normalization  
- CNN-based model design and training  
- Model evaluation using accuracy and loss metrics  

## Results
The model was evaluated using accuracy 77 % and loss metrics.
Ongoing experimentation and hyperparameter tuning are being conducted to improve model accuracy.


## Notes
This project is intended for academic and learning purposes.

