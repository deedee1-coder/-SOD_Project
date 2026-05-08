
# Salient Object Detection Using CNN Encoder-Decoder Networks

## Project Overview

This project implements a Salient Object Detection (SOD) system using Convolutional Neural Networks built entirely from scratch with PyTorch. The goal of the project is to identify and segment the most visually important object or region within an image by generating a saliency mask.

The project covers the complete deep learning workflow, including:

- Dataset preparation and preprocessing
- Data augmentation
- CNN encoder-decoder model design
- Model training and validation
- Performance evaluation using segmentation metrics
- Visualization of predicted saliency masks
- Interactive demo for inference on custom images

Two models were implemented:
1. Baseline CNN model
2. Improved CNN model using Batch Normalization and Dropout

---

# Dataset

The project uses the DUTS Saliency Detection Dataset.

Dataset Source:
https://www.kaggle.com/datasets/balraj98/duts-saliency-detection-dataset

Dataset Information:
- 10,553 training images
- 5,019 testing images
- Pixel-level saliency masks
- Challenging object segmentation scenarios

---

# Technologies Used

- Python 3
- PyTorch
- OpenCV
- NumPy
- Matplotlib
- scikit-learn
- Google Colab

---

# Project Structure

```text
├── demo_notebook.ipynb
├── Project_Report.pdf
├── Presentation_Slides.pptx
├── best_improved_sod_model.pth
├── dataset/
└── README.md
````

---

# Features

* Image preprocessing and normalization
* Data augmentation techniques
* Encoder-decoder CNN architecture
* Improved CNN with BatchNorm and Dropout
* BCE + IoU combined loss function
* Early stopping and best model saving
* IoU, Precision, Recall, and F1-score evaluation
* Overlay visualization of predicted masks
* Demo for custom image inference

---

# Model Architecture

## Baseline CNN

* Conv2D layers
* ReLU activations
* MaxPooling layers
* ConvTranspose2D decoder
* Sigmoid output mask

## Improved CNN

* Batch Normalization
* Dropout regularization
* Increased feature channels
* Improved training stability

---

# Evaluation Metrics

The models were evaluated using:

* Intersection-over-Union (IoU)
* Precision
* Recall
* F1-Score

---

# Demo

The notebook includes a demo section where users can:

1. Upload a custom image
2. Generate a saliency mask
3. Visualize overlay predictions
4. Measure inference time

---

# Results

The baseline CNN successfully learned salient object regions and generated meaningful segmentation masks.

Example metrics achieved by the baseline model:

| Metric    | Score  |
| --------- | ------ |
| IoU       | 0.4704 |
| Precision | 0.6235 |
| Recall    | 0.6938 |
| F1 Score  | 0.6077 |

---

# How to Run

## Option 1 — Google Colab

1. Open `demo_notebook.ipynb`
2. Upload the DUTS dataset
3. Run notebook cells sequentially
4. Train the model or load saved weights
5. Run the demo section

---

# Author

Project developed as part of an End-to-End Machine Learning / Deep Learning project on Salient Object Detection.

```
```
