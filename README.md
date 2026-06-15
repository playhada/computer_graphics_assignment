# Computer Graphics Assignment

This repository contains Python implementations of image processing and machine learning assignments for the Computer Graphics course.

---

## Project Structure
computer_graphics_assignment/

│

├── image_arithmetic_operations.py     # Assignment 2: Arithmetic Operations

├── histogram_enhancement.py           # Assignment 1: Histogram-based Enhancement

├── knn_assignment.py                  # Assignment 3: K-Nearest Neighbor

└── linear_classification.py           # Assignment 4: Linear Classification

---

## 📌 Assignment 1: Histogram-based Image Enhancement

Applies three histogram enhancement techniques to a grayscale image and evaluates each with image quality metrics.

**Techniques applied:**
- Histogram Equalization (HE)
- Adaptive Histogram Equalization (AHE)
- Contrast Limited Adaptive Histogram Equalization (CLAHE)

**Evaluation Metrics:** MSE / PSNR / SSIM

**How to run:**
```bash
pip install opencv-python numpy matplotlib scikit-image
python histogram_enhancement.py
```

> Image is downloaded automatically via `urllib`.

---

## 📌 Assignment 2: Arithmetic Operations on Images

Performs various arithmetic and bitwise operations between two images.

**Operations included:**
- Addition (`cv2.add`, NumPy clip)
- Subtraction (`cv2.subtract`)
- Blending (`cv2.addWeighted`, α sweep: 0.0 → 1.0)
- Multiplication / Division
- Bitwise AND / OR / XOR / NOT

**How to run:**
```bash
pip install opencv-python numpy matplotlib
python image_arithmetic_operations.py
```

> Two sample images (landscape + Lena) are downloaded automatically.

---

## 📌 Assignment 3: K-Nearest Neighbor Classification

Implements KNN from scratch on CIFAR-10 with 5-fold cross-validation.

**Key features:**
- L1 / L2 distance metrics
- K values: [1, 3, 5, 7, 9]
- Cross-validation accuracy plot
- Confusion matrix visualization

**How to run:**
```bash
pip install numpy matplotlib
python knn_assignment.py
```

> CIFAR-10 dataset is downloaded automatically (~163MB).

---

## 📌 Assignment 4: Linear Classification

Implements SVM (Hinge Loss) and Softmax (Cross-Entropy Loss) linear classifiers from scratch on CIFAR-10.

**Key features:**
- Mini-batch Gradient Descent
- Bias trick (bias absorbed into W)
- L2 regularization
- Loss curve comparison (SVM vs Softmax)
- Learned weight template visualization per class

**How to run:**
```bash
pip install numpy matplotlib
python linear_classification.py
```

> CIFAR-10 dataset is downloaded automatically (~163MB).

---

## Requirements
opencv-python

numpy

matplotlib

scikit-image

Install all at once:
```bash
pip install opencv-python numpy matplotlib scikit-image
```

---

## Environment

- Python 3.x
- Google Colab / Jupyter Notebook
