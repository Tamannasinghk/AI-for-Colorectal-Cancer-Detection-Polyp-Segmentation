# 🏥 AI for Colorectal Cancer Detection: Polyp Segmentation

![Polyp Segmentation Example](https://media.springernature.com/lw685/springer-static/image/art%3A10.1007%2Fs10278-023-00954-2/MediaObjects/10278_2023_954_Fig1_HTML.jpg)  
*Example of AI segmenting polypsin colonoscopy images*

## 🚀 Overview
This project develops a **deep learning system to detect colorectal cancer precursors (polyps)** in colonoscopy images using:
- **U-Net with EfficientNet-B4 backbone** (transfer learning)
- **Dice + Focal Loss** for handling class imbalance
- **T4 GPU-accelerated training** (Google Colab)

**Achieves 70%+ Dice Score** - comparable to clinical-grade performance!

## 📋 Dataset
We use the **[Kvasir-SEG](https://datasets.simula.no/kvasir-seg/)** dataset:
- 1,000 high-resolution colonoscopy images
- Expert-annotated polyp segmentation masks
- Samples with varying polyp sizes/shapes

## 🛠️ Tech Stack
| Component               | Technology |
|-------------------------|------------|
| **Deep Learning**       | PyTorch, Segmentation Models PyTorch |
| **Image Processing**    | OpenCV, Albumentations |
| **GPU Acceleration**    | Google Colab (T4 GPU) |
| **Model Interpretability** | Grad-CAM |

## 📂 Repository Structure
```bash
   .
   ├── notebooks/
   │ └── colorectal_cancer_prediction.ipynb # Full training pipeline
   ├── models/
   │ └── best_model.pth #Please train by yourself , model can not be uploaded here because of size .
   └── README.md
```

## 🚀 Quick Start
1. **Run in Google Colab**:  
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Tamannasinghk/AI-for-Colorectal-Cancer-Detection-Polyp-Segmentation/blob/main/notebooks/colorectal_cancer_prediction.ipynb)

2. **Local Installation**:
   ```bash
   git clone https://github.com/Tamannasinghk/AI-for-Colorectal-Cancer-Detection-Polyp-Segmentation
   cd AI-for-Colorectal-Cancer-Detection-Polyp-Segmentation
   ```
## 🏆 Key Features
✔ Hybrid U-Net Architecture with SCSE attention

✔ Dynamic Thresholding during validation

✔ OneCycleLR for fast convergence

✔ Grad-CAM explainability maps

---
## Thankyou
