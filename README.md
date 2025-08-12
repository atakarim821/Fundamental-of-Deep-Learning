# Image Captioning using NetVLAD

This project implements an **Image Captioning** system using a **NetVLAD layer** for image feature aggregation, completed as part of the **Fundamentals of Deep Learning (CS6910)** course at IIT Madras.

## 📌 Overview
Image Captioning is the task of generating a textual description for an image.  
In this project, we:
- Extract visual features from images using a CNN encoder.
- Use **NetVLAD** to aggregate features for improved global image representation.
- Employ an LSTM decoder to generate captions from the aggregated features.
- Train and evaluate the model on the **Flickr8k** dataset.

## 🚀 Features
- **NetVLAD layer** for robust feature aggregation, improving performance on diverse scenes.
- Batch generator to handle large datasets efficiently without exhausting memory.
- BLEU score evaluation for caption quality.

## 📊 Dataset
- **Flickr8k** dataset: 8,000 images with five captions each.
- Preprocessed with tokenization and padding for LSTM input.

## 🏆 Results
- Achieved **BLEU-4 score of ~0.32** on the Flickr8k test set.
- Demonstrated better performance compared to standard mean-pooled feature approaches.

## ⚙️ Requirements
- Python 3.x
- TensorFlow / Keras
- NumPy, Pandas
- Git LFS (for large files)

## 📂 Project Structure
FoDL/
│── caption/ # Scripts and utilities
│── flickr8k/ # Dataset files
│── image_features.pkl # Precomputed image features
│── model_lstm.h5 # Trained model
│── caption.ipynb # Main notebook
│── README.md

