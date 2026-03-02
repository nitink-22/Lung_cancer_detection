# 🫁 Lung Cancer Detection using CNN

### 🔬 Project Overview
This project leverages **Deep Learning** to automate the detection of lung cancer from histopathological images. By utilizing a **Convolutional Neural Network (CNN)**, the model classifies tissue samples into three distinct diagnostic categories with high precision.

---

## 📂 Repository Structure
```bash
├── lung_colon_image_set/
│   ├── lung_image_sets/
│   │   ├── lung_aca/   # Adenocarcinoma
│   │   ├── lung_n/     # Benign tissue
│   │   └── lung_scc/   # Squamous cell carcinoma
├── code_file.ipynb     # Main Jupyter Notebook
└── README.md           # Project Documentation
```
🧠 Model Architecture


The model is built using a Sequential API with a focus on hierarchical feature extraction:
Input Layer: 128 x 128 x 3 RGB images.
Preprocessing: Rescaling layer to normalize pixel values to [0, 1].

Feature Extraction:
Conv2D (32 filters) + MaxPooling2D.
Conv2D (64 filters) + MaxPooling2D.

Classification: Flatten layer followed by a Dense output layer with 3 units.



📈 Performance Results




The model was trained over 10 epochs, showing consistent improvement in both training and validation sets.



🚀 Final Test Accuracy: 90.80%


📉 Final Test Loss: 0.3340





🛠️ Tech Stack




Language: Python


Libraries: TensorFlow, Keras, NumPy, Scikit-Learn


Visualization: Matplotlib


Environment: Jupyter Notebook / VS Code



---

## ✍️ Author
**Nitin Kumar** 

*Machine Learning Student* 
