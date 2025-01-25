# COVID-19 Image Classification

This project uses deep learning to classify COVID-19 and non-COVID-19 cases from chest X-ray images. It leverages a pre-trained MobileNet model fine-tuned on a custom dataset. The implementation is built with PyTorch, and the application is deployed through a web interface using Streamlit.

---

## Table of Contents
- [About the Project](#about-the-project)
- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Example Output](#example-output)

---

## About the Project
The **COVID-19 Image Classification** project is designed to assist in:
- **Classification of Chest X-rays**: Distinguishing between COVID-19 positive and negative cases based on X-ray images.

The model leverages MobileNet, a lightweight and efficient convolutional neural network, pre-trained on ImageNet and fine-tuned on a dataset of chest X-rays. PyTorch is the main library used for the implementation.

---

## Features
- **Image Preprocessing**: Resizes, normalizes, and augments input images for improved performance.
- **COVID-19 Classification**: Identifies whether the X-ray image indicates a COVID-19 infection.
- **Web Application**: Provides an easy-to-use interface for uploading images and viewing predictions.
- **Explainability**: Optionally generates Grad-CAM visualizations to highlight regions influencing the model's decisions.

---

## Getting Started

Follow these steps to set up and run the project locally:

### Prerequisites
- Python 3.8+
- PyTorch (1.8.0+ recommended)
- Pre-trained MobileNet model file (`mobilenet_covid19.pt`)

---

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-link>
   cd covid19_image_classification
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure the pre-trained model is in the project directory:
   - `mobilenet_covid19.pt`: Fine-tuned MobileNet model for COVID-19 classification.

---

## Project Structure
The project files are organized as follows:
```
covid19_image_classification/
├── training/
│   ├── dataset_preparation.py   # Script for data preprocessing
│   ├── train_mobilenet.py       # Training script for MobileNet
│   └── mobilenet_covid19.pt     # Pre-trained MobileNet model
├── utils.py                     # Utility functions for image preprocessing and Grad-CAM
└── README.md                    # Project documentation
```

