Skin Cancer Detection using CNN (Deep Learning)


Overview:

This project applies Convolutional Neural Networks (CNN) to classify skin lesions as Benign or Malignant using dermoscopic images. It demonstrates how deep learning can assist in early cancer detection through automated medical image analysis.

The model is trained using TensorFlow/Keras with data augmentation, learning rate scheduling, and early stopping to achieve strong generalization and prevent overfitting.

Features:

Binary classification for skin cancer detection

Custom CNN architecture built from scratch

Data preprocessing and augmentation using ImageDataGenerator

Visualization of model accuracy, loss, and confusion matrix

Model evaluation with precision, recall, and F1‑score

Single‑image testing with result visualization

Dataset:

Dataset used: ISIC / HAM10000

Structure:

text
dataset/
├── train/
│   ├── Benign/
│   └── Malignant/
└── test/
    ├── Benign/
    └── Malignant/
Training images: 11,879

Testing images: 2,000

Image resolution: 224×224

Model Architecture:

Model Type: Sequential CNN
Layers:

Conv2D (32 filters) + MaxPooling

Conv2D (64 filters) + MaxPooling

Conv2D (128 filters) + MaxPooling

Flatten + Dense(512) + Dropout(0.5)

Output Dense(1, Sigmoid)

Optimizer: Adam
Loss: Binary Cross‑Entropy
Callbacks: EarlyStopping, ReduceLROnPlateau

Accuracy and Results:

Training Accuracy: ~90%

Validation Accuracy: ~88%

Validation Loss: 0.29

Precision & Recall: ≈ 0.52 each (Test Set)

Visualization outputs include:

Accuracy–loss graph

Confusion matrix heatmap

Image‑wise predictions displaying Benign or Malignant status
