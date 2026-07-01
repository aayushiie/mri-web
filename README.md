# MRI Tumor Detection System

A Flask-based web application that classifies brain MRI scans into one of four categories using a fine-tuned VGG16 convolutional neural network.

## Features

- Upload brain MRI images through a simple web interface
- Detects one of four classes:
  - Glioma
  - Meningioma
  - Pituitary Tumor
  - No Tumor
- Displays prediction confidence
- Downloads the trained model automatically from Hugging Face during deployment

## Tech Stack

- Python
- Flask
- TensorFlow / Keras
- VGG16 (Transfer Learning)
- Bootstrap 5

## Running Locally

```bash
pip install -r requirements.txt
python main.py
```

Open:

```
http://127.0.0.1:5000
```

## Model

The trained VGG16 model is hosted on Hugging Face:

**Repository:** https://huggingface.co/aayushiie/brain-tumor-cnn

The application downloads the model automatically on first startup.

## Dataset

The model was trained on a brain MRI dataset containing four classes:

- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor
