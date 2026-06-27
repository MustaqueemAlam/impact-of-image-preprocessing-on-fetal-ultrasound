# 🩺 Evaluating the Impact of Image Preprocessing on Deep Learning-Based Fetal Ultrasound Classification under Class Imbalance

Official implementation of our conference paper.

---

## 📖 Overview

This repository contains the Google Colab notebooks used to evaluate the impact of different image preprocessing techniques on deep learning-based fetal ultrasound classification using **ResNet-50**.

Three preprocessing pipelines were investigated under identical experimental settings:

- Baseline (Zero Padding)
- Prewitt Filter + Zero Padding
- Gamma Correction + Zero Padding

The experiments were implemented using **TensorFlow/Keras** and executed on **Google Colab GPU**.

---

## 📂 Repository Structure

```
.
├── Baseline_Preprocessing.ipynb
├── Prewitt_Filter_Preprocessing.ipynb
├── Gamma_Correction_Preprocessing.ipynb
├── README.md
├── requirements.txt
└── LICENSE
```

---

# 📓 Notebooks

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

# 💻 Development Environment

The experiments were conducted using:

- Google Colab
- Python 3.x
- TensorFlow 2.x
- Keras
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn

GPU Used:

- NVIDIA Tesla T4 (Google Colab)

---

# 📂 Dataset

The experiments utilize the **Ultrasound Fetus Dataset**.

Classes:

- Normal
- Benign
- Malignant

Total Images:

- 1669

The dataset is **not included** in this repository due to licensing restrictions.

Please download it from its official source and update the dataset path inside each notebook.

Dataset link: https://www.kaggle.com/datasets/orvile/ultrasound-fetus-dataset

---

# 🚀 Running the Notebooks

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

# 📊 Experimental Pipelines

### Notebook 1

Baseline

- Resize
- Zero Padding
- Transfer Learning
- Fine-tuning

---

### Notebook 2

Prewitt Filter

- Edge Detection
- Zero Padding
- Transfer Learning
- Fine-tuning

---

### Notebook 3

Gamma Correction

- Gamma Enhancement
- Zero Padding
- Transfer Learning
- Fine-tuning

---

# 📈 Main Results

| Pipeline | Accuracy | Macro F1 |
|-----------|---------:|----------:|
| Baseline | 0.63 | 0.44 |
| Prewitt | **0.64** | 0.45 |
| Gamma Correction | 0.63 | **0.46** |

The results indicate that image preprocessing may provide marginal improvements, while dataset imbalance remains the dominant challenge.

---

# 📄 License

This repository is released under the MIT License.

---

# ⚠️ Disclaimer

This repository is intended solely for academic research and educational purposes. It is **not intended for clinical diagnosis or medical decision-making.**
