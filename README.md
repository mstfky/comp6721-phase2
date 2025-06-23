# COMP6721 – Phase 2: Indoor Venue Classification with CNN (PyTorch)

This project implements a Convolutional Neural Network (CNN) from scratch using PyTorch to classify indoor scene images into three categories:

- 📚 `library-indoor`
- 🖼️ `museum-indoor`
- 🛍️ `shopping_mall-indoor`

---

## 📁 Dataset
The dataset was provided in two folders:
- `Training/` – containing subfolders for each class.
- `Test/` – used for final evaluation.

Images were resized to **128×128**, normalized, and split into **training and validation** sets (80/20 split).

---

## 🧠 Model Architecture
A scratch-built CNN consisting of:
- 3 convolutional layers (ReLU + MaxPool)
- 2 fully connected layers
- Dropout for regularization
- CrossEntropyLoss for training

---

## 🔍 Hyperparameter Tuning
Grid search was performed over:
- Learning rates: `0.001`, `0.0001`
- Batch sizes: `32`, `64`

Best validation accuracy: **77.97%** with `LR=0.001` and `BS=64`.

---

## 📊 Final Results
- ✅ **Test Accuracy:** 70%
- Metrics include: precision, recall, F1-score
- Visualized via a confusion matrix

---

## 📦 Files
- `phase2.ipynb` – Complete Colab notebook with code, training, evaluation, and results
- `README.md` – Project summary

---

## ▶️ Demo
Model saved as `best_model.pth` and supports live testing with unseen images.

---

## 🛠️ Future Improvements
- Data augmentation
- Transfer learning (e.g., using ResNet)
- Hyperparameter tuning via tools like Optuna

