Lung Cancer Detection using CNN

This project implements a Convolutional Neural Network (CNN) to automate the detection of lung cancer from histopathological images. By analyzing microscopic tissue patterns, the model classifies samples into three distinct categories with high accuracy.

📌 Project Overview

The objective of this project is to provide a deep learning-based tool to assist pathologists in diagnosing lung cancer. The model is trained to distinguish between healthy tissue and the two most common types of lung carcinoma.

Key Features:

Automated Classification: Classifies tissue slides into 3 categories.

High Accuracy: Achieved a 90.80% accuracy on the unseen testing dataset.

Efficient Processing: Uses image resizing and batch processing to handle large medical datasets on standard hardware.

📊 Dataset

The project utilizes the LC25000 Histopathological Dataset.

Total Lung Images: 15,000 images.

Classes:
1. lung_aca: Lung Adenocarcinoma.
2. lung_n: Benign Lung Tissue.
3. lung_scc: Lung Squamous Cell Carcinoma.

Image Specs: Original images are 768×768 pixels, resized to 128×128 for the model.

🛠️ Tech Stack
Language: Python

Deep Learning: TensorFlow / Keras

Data Handling: NumPy, Scikit-Learn

Visualization: Matplotlib

Environment: Jupyter Notebook / VS Code

🧠 Model Architecture
The model is a Sequential CNN built with the following layers:


Input Layer: 128×128×3 RGB images.

Rescaling: Normalizes pixel values from [0,255] to [0,1].

Convolutional Layers: Two stages of Conv2D (32 and 64 filters) to extract microscopic textures.

Pooling Layers: MaxPooling2D to reduce spatial dimensions and focus on key features.

Flatten & Output: A Dense layer with 3 units for final classification.

📈 Results
The model was trained for 10 epochs, showing a steady increase in both training and validation accuracy.

Metric	Score

Final Test Accuracy	90.80%
Final Test Loss	0.3340

📁 Repository Structure

├── lung_colon_image_set/
│   ├── lung_image_sets/
│   │   ├── lung_aca/
│   │   ├── lung_n/
│   │   └── lung_scc/
├── code_file.ipynb
└── README.md
