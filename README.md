# Flower Image Classification Project

## Overview

This project implements a Convolutional Neural Network (CNN) using TensorFlow/Keras to classify images of various flower types. The model is trained on a flower dataset and converted into multiple formats for deployment on different platforms including TensorFlow SavedModel, TensorFlow.js, and TensorFlow Lite.

---

## Project Structure



## Project Structure
```bash
flowers-image-classification/
│
├── saved_model/ # TensorFlow SavedModel format files
├── tfjs_model/ # TensorFlow.js model files for web deployment
├── tflite/ # TensorFlow Lite model and labels for mobile/embedded devices
├── klasifikasi_bunga_cnn.py # Main Python script for training and inference
├── klasifikasi_bunga_cnn.ipynb
├── requirements.txt # Python dependencies
├── README.md # Project documentation (this file)
└── .gitignore # Files to ignore in git commit
```

---

## Data Preparation

- The dataset consists of images grouped by flower classes.
- Data is split into training, validation, and test sets.
- Image augmentation is applied during training to improve generalization.

---

## Model Architecture

- Utilizes a CNN model built with TensorFlow Keras `Sequential` API.
- Contains multiple `Conv2D` and `MaxPooling2D` layers for feature extraction.
- Followed by `Dropout` and dense layers to reduce overfitting and perform classification.
- Uses `softmax` activation in output layer corresponding to number of flower classes.

---

## Training

- Training includes callbacks such as Early Stopping and Learning Rate Scheduler for optimization.
- Model training progress is visualized with graphs for accuracy and loss.
- Final evaluation includes accuracy score and confusion matrix visualization.

---

## Conversion and Export

- Model converted and saved in three formats:
  - **SavedModel** for TensorFlow deployment.
  - **TensorFlow.js** format for web apps.
  - **TensorFlow Lite** format with label file for mobile and embedded uses.

---

## How to Run

1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Train or run inference:

```bash
python klasifikasi_bunga_cnn.py
```
Make sure the script and the model folders (saved_model, tfjs_model, tflite) are in the same root project directory.

## Results

- Training and validation accuracy reach satisfactory levels (refer to training plots).
- Confusion matrix shows the performance per class.
- Model size is optimized with TensorFlow Lite for mobile deployment.

## License

MIT License 

## Author

Gymnastiar Harun 📧 gimnastiarhrn@gmail.com 🔗 LinkedIn [www.linkedin.com/in/gymnastiarharun]