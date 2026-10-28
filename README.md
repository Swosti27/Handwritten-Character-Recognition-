# Handwritten Character Recognition using CNN (MNIST & EMNIST)

## 📌 Project Overview

This project implements a **Handwritten Digit and Character Recognition system** using **Convolutional Neural Networks (CNNs)**.  
The model is first trained on the **MNIST digit dataset** and then extended to recognize **handwritten English uppercase letters (A–Z)** using the **EMNIST Letters dataset** loaded via **TensorFlow Datasets (TFDS)**.

The system demonstrates how deep learning models can automatically extract spatial features from handwritten images and achieve high accuracy in image classification tasks.

---

## 🎯 Objectives

- Build a CNN model for handwritten digit recognition  
- Extend the model for handwritten character recognition (A–Z)  
- Apply preprocessing and data augmentation  
- Evaluate model performance using accuracy and confusion matrix  
- Test the model on custom handwritten images  

---

## 🧠 Technologies Used

- Python  
- TensorFlow / Keras  
- TensorFlow Datasets (TFDS)  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- OpenCV  

---

## 📂 Project Structure
Project_Structure/
│
├── notebooks/
│ └── Handwritten_CNN.ipynb
│
├── models/
│ ├── mnist_cnn_model.keras
│ └── emnist_character_cnn_tfds_final.keras
│
├── sample_inputs/
│ ├── digit.png
│ └── char.png
│
├── output/
│ ├── prediction.txt
│ ├── training_accuracy.png
│ ├── training_loss.png
│ └── confusion_matrix.png
│
├── report/
│ └── Handwritten_Character_Recognition_Report.pdf
│
├── requirements.txt
└── README.md
---

## 📊 Datasets Used

### 1️⃣ MNIST Dataset
- Handwritten digits (0–9)  
- 60,000 training images  
- 10,000 test images  
- Image size: 28 × 28 grayscale  

### 2️⃣ EMNIST Letters Dataset (via TFDS)
- Handwritten uppercase letters (A–Z)  
- 88,800 training images  
- 14,800 test images  
- Image size: 28 × 28 grayscale  

> **Note:**  
> TensorFlow Datasets (TFDS) is used instead of the `emnist` package for better stability and compatibility.

---

## ⚙️ Installation & Setup

### Step 1: Create a virtual environment (recommended)

```bash
conda create -n hcr python=3.10 -y
conda activate hcr
```
### Step 2: Install dependencies
```bash
pip install -r requirements.txt
```

## 🚀 How to Run the Project (Day-wise)

### 🔹 Day 1: MNIST Digit Recognition
**Notebook:** `Day1_MNIST_CNN.ipynb`

- Load MNIST dataset  
- Normalize and reshape images  
- Build CNN architecture  
- Train and evaluate digit recognition model  
- Save trained model  

---

### 🔹 Day 2: Evaluation & Testing
**Notebook:** `Day2_Evaluation.ipynb`

- Plot training and validation curves  
- Generate confusion matrix  
- Test model on individual MNIST digits  
- Handle overfitting using dropout  

---

### 🔹 Day 3: EMNIST Character Recognition (TFDS)
**Notebook:** `Day3_EMNIST_TFDS.ipynb`

- Load EMNIST Letters using TensorFlow Datasets (TFDS)  
- Fix image orientation  
- Normalize and reshape images  
- Modify CNN for 26 classes (A–Z)  
- Train character recognition model  

---

### 🔹 Day 4: Model Improvement & Evaluation
**Notebook:** `Day4_Improvement_Evaluation.ipynb`

- Apply data augmentation  
- Use EarlyStopping to prevent overfitting  
- Retrain the model  
- Generate and save:
  - Training curves  
  - Confusion matrix  
  - Classification report  

---

### 🔹 Day 5: Final Demo & Custom Prediction
**Notebook:** `Day5_Final_Demo.ipynb`

- Load final trained model  
- Predict multiple test characters  
- Predict custom handwritten character images  
- Save prediction output  
- Final project summary  

---

## 🖼️ Custom Image Testing

To test your own handwritten character:

1. Place the image in `sample_inputs/char.png`  
2. The image should contain:
   - One uppercase character  
   - Clear background  
3. Run the **Day 5 notebook**  
4. The model predicts the character  

---

## 📈 Results

- **MNIST Digit Accuracy:** ~98%  
- **EMNIST Character Accuracy:** ~88–90%  
- Data augmentation improved generalization  
- Confusion matrix shows misclassification among similar characters  

---

## 🧠 Key Learnings

- CNNs are highly effective for image-based classification  
- Proper preprocessing is critical for correct predictions  
- Data augmentation improves robustness  
- Evaluation metrics beyond accuracy are essential  

---

## 🔮 Future Scope

- Word-level recognition using CRNN + CTC loss  
- Support for lowercase letters and digits  
- Real-time OCR using webcam  
- Multilingual character recognition  

---

## 👨‍🎓 Author

**Name:** Swosti Deepan Sahoo  
**Project Type:** Machine Learning Project  
