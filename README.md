# 🩺 Evaluating the Impact of Image Preprocessing on Deep Learning-Based Fetal Ultrasound Classification under Class Imbalance

---

## 📖 Overview

This repository contains the official implementation of our research on evaluating the impact of image preprocessing techniques for deep learning-based fetal ultrasound image classification using **ResNet-50**.

Three preprocessing pipelines were investigated under identical experimental settings:

- Baseline (Zero Padding)
- Prewitt Filter + Zero Padding
- Gamma Correction + Zero Padding

The experiments were implemented using **TensorFlow/Keras** and executed on **Google Colab GPU**. The complete implementation is provided through three Jupyter notebooks.

---

## 📄 Research Paper

**Title**

> *Evaluating the Impact of Image Preprocessing on Deep Learning-Based Fetal Ultrasound Classification under Class Imbalance*

**Conference**

**ICICDS 2026** (International Conference on Intelligent Computing, Information and Communication Systems)

**Publication Status**

Presented at **ICICDS 2026**.

The paper has been accepted for publication in the **ICICDS 2026 Conference Proceedings** and will be published soon.

---

## 📂 Repository Structure

```text
.
├── Baseline_Preprocessing.ipynb
├── Prewitt_Filter_Preprocessing.ipynb
├── Gamma_Correction_Preprocessing.ipynb
├── README.md
```

---

## 📓 Notebooks

| Notebook | Description |
|-----------|-------------|
| `Baseline_Preprocessing.ipynb` | Training ResNet-50 using zero-padded ultrasound images (baseline). |
| `Prewitt_Filter_Preprocessing.ipynb` | Applies Prewitt edge enhancement before model training. |
| `Gamma_Correction_Preprocessing.ipynb` | Applies gamma correction before model training. |

Each notebook contains:

- Dataset loading
- Image preprocessing
- Data augmentation
- Transfer learning
- Fine-tuning
- Evaluation metrics
- ROC Curve
- Confusion Matrix
- Grad-CAM visualization

---

## 💻 Development Environment

The experiments were conducted using:

- Google Colab
- Python 3.x
- TensorFlow 2.x
- Keras
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn

**GPU Used**

- NVIDIA Tesla T4 (Google Colab)

---

## 📂 Dataset

The experiments utilize the **Ultrasound Fetus Dataset**.

**Classes**

- Normal
- Benign
- Malignant

**Total Images**

- 1,669

The dataset is **not included** in this repository due to licensing restrictions.

Please download it from its official source and update the dataset path inside each notebook.

**Dataset**

https://www.kaggle.com/datasets/orvile/ultrasound-fetus-dataset

---

## 🚀 Running the Notebooks

1. Clone the repository

```bash
git clone https://github.com/MustaqueemAlam/impact-of-image-preprocessing-on-fetal-ultrasound.git
```

2. Open any notebook using:

- Google Colab
- Jupyter Notebook
- JupyterLab

3. Mount Google Drive (if using Colab).

4. Update the dataset directory.

5. Run all cells sequentially.

---

## 📊 Experimental Pipelines

### Baseline

- Resize
- Zero Padding
- Transfer Learning
- Fine-tuning

### Prewitt Filter

- Edge Detection
- Zero Padding
- Transfer Learning
- Fine-tuning

### Gamma Correction

- Gamma Enhancement
- Zero Padding
- Transfer Learning
- Fine-tuning

---

## 📈 Main Results

| Pipeline | Accuracy | Macro F1 |
|-----------|---------:|----------:|
| Baseline | 0.63 | 0.44 |
| **Prewitt Filter** | **0.64** | 0.45 |
| Gamma Correction | 0.63 | **0.46** |

The results indicate that image preprocessing provides only marginal performance improvements, while severe class imbalance remains the primary factor limiting classification performance.

---

## 📄 License

This project is released under the **MIT License**.

---

## ⚠️ Disclaimer

This repository is intended solely for academic research and educational purposes. It is **not intended for clinical diagnosis or medical decision-making.**
