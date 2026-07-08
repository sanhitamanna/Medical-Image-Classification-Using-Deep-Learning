# Medical-Image-Classification-Using-Deep-Learning
# CT Brain Tumor Classification Using Deep Learning

## Overview

This project implements an end-to-end deep learning framework for **CT Brain Tumor Classification** using **TensorFlow**, **Keras**, and **OpenCV**. The objective is to automatically classify brain CT images into **Tumor** and **Normal** categories, assisting computer-aided diagnosis (CAD) systems in medical imaging.

The framework utilizes **EfficientNetB0** as a transfer learning backbone for robust feature extraction, along with image preprocessing and data augmentation techniques to improve classification performance.

---

## Features

* End-to-end deep learning pipeline
* CT brain image preprocessing
* Image resizing and normalization
* Data augmentation
* Transfer learning using EfficientNetB0
* Binary classification (Tumor / Normal)
* Model training and validation
* Performance evaluation
* Single-image prediction
* Model checkpointing and early stopping

---

## Technologies Used

* Python
* TensorFlow 2.x
* Keras
* OpenCV
* NumPy
* Matplotlib
* Scikit-learn

---

## Project Structure

```text
CT_Brain_Tumor_Classification/
│
├── dataset/
│   ├── train/
│   │   ├── Normal/
│   │   └── Tumor/
│   │
│   ├── validation/
│   │   ├── Normal/
│   │   └── Tumor/
│   │
│   └── test/
│       ├── Normal/
│       └── Tumor/
│
├── train.py
├── predict.py
├── evaluate.py
├── requirements.txt
├── README.md
└── best_model.keras
```

---

## Dataset Structure

The dataset should be organized as follows:

```text
dataset/
│
├── train/
│   ├── Normal/
│   └── Tumor/
│
├── validation/
│   ├── Normal/
│   └── Tumor/
│
└── test/
    ├── Normal/
    └── Tumor/
```

Each folder should contain CT brain images in one of the following formats:

* `.jpg`
* `.jpeg`
* `.png`

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/CT-Brain-Tumor-Classification.git
```

Navigate to the project folder:

```bash
cd CT-Brain-Tumor-Classification
```

Install the required packages:

```bash
pip install -r requirements.txt
```

---

## Required Libraries

```text
tensorflow
opencv-python
numpy
matplotlib
scikit-learn
pandas
```

---

## Model Architecture

The proposed model consists of:

```
Input CT Image (224 × 224)

↓

Image Preprocessing

↓

Data Augmentation

↓

EfficientNetB0 (Pre-trained)

↓

Global Average Pooling

↓

Dense Layer

↓

Dropout

↓

Sigmoid Classifier

↓

Prediction
```

---

## Training

Run:

```bash
python train.py
```

The training process includes:

* Image preprocessing
* Data augmentation
* Model training
* Validation
* Early stopping
* Model checkpointing

---

## Evaluation

The trained model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Example:

| Metric    | Value |
| --------- | ----: |
| Accuracy  | 92.3% |
| Precision | 92.1% |
| Recall    | 93.0% |
| F1-score  | 92.5% |

> **Note:** Actual results will depend on the dataset used, its size, and the training configuration.

---

## Predict a New CT Image

Run:

```bash
python predict.py
```

The model predicts whether the input CT image belongs to:

* Normal
* Tumor

---

## Results

The trained model generates:

* Training accuracy curve
* Validation accuracy curve
* Loss curve
* Confusion matrix
* Classification report

---

## Future Improvements

* Multi-class brain tumor classification
* Explainable AI using Grad-CAM
* Hyperparameter optimization
* Cross-validation
* Deployment using Flask or FastAPI
* Docker containerization
* TensorBoard experiment tracking

---

## Applications

* Computer-Aided Diagnosis (CAD)
* Clinical decision support
* Medical image analysis
* Healthcare AI research
* Educational and research projects

---

## License

This project is released under the MIT License. You are free to use, modify, and distribute it with appropriate attribution.

---

## Citation

If you use this repository in your research or academic work, please cite the repository appropriately and reference the associated publication (if available).

---

## Author

**Sanhita Manna**

Assistant Professor

Research Interests:

* Medical Image Processing
* Artificial Intelligence
* Deep Learning
* Computer Vision
* Biomedical Signal Processing
