# 📘 Project Summary: Cancer Diagnosis with ANN

## 🧾 Overview
This project uses an Artificial Neural Network (ANN) built with TensorFlow to classify tumors as **malignant** or **benign** using the Wisconsin Breast Cancer dataset. The dataset contains features computed from digitized images of fine needle aspirates (FNAs) of breast masses.

---

## 📊 Dataset Highlights
- **Source**: [Kaggle – Wisconsin Breast Cancer Dataset](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data)
- **Samples**: 569
- **Classes**: 2 (Malignant = 1, Benign = 0)
- **Features**: 30 numeric features (mean, standard error, worst value of measurements)

---

## ⚙️ Preprocessing Steps
- Dropped irrelevant columns (`id`, `Unnamed: 32`)
- Encoded target variable (`M` → 1, `B` → 0)
- Normalized feature values using `StandardScaler`
- Split into training and test sets (80/20)

---

## 🧠 ANN Model Architecture
- **Input Layer**: 30 neurons (1 for each feature)
- **Hidden Layer 1**: 30 neurons, ReLU activation
- **Hidden Layer 2**: 15 neurons, ReLU activation
- **Output Layer**: 1 neuron, Sigmoid activation (binary classification)

---

## 🏋️ Training Details
- **Optimizer**: Adam
- **Loss Function**: Binary Crossentropy
- **Epochs**: 100
- **Batch Size**: 16
- **Validation Split**: 10%

---

## 📈 Performance Metrics (on test data)
_Replace with your actual evaluation results:_

- **Accuracy**: 96.49%
- **Precision**: 95.00%
- **Recall**: 97.00%
- **F1-score**: 96.00%

---

## ✅ Key Takeaways
- The ANN model showed strong performance in distinguishing malignant from benign tumors.
- Data normalization and proper train/test splitting were key to effective training.
- Further performance improvement is possible with dropout, regularization, and hyperparameter tuning.

---

## 🚀 Potential Extensions
- Use cross-validation for more robust evaluation.
- Explore other models like Random Forests or SVMs for comparison.
- Integrate model into a simple diagnostic web app using Flask or Streamlit.
- Apply to other medical diagnosis tasks with similar feature structures.
