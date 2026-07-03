# 🌊 Underwater Image Enhancement (UIE) using CNN

A deep learning project to enhance degraded underwater images using a **Convolutional Neural Network (CNN)**, built on the UIEB dataset.

> Developed as part of Summer Research Internship at **NIT Karnataka, Surathkal**  
> Under the guidance of **Dr. Jidesh P.**, Department of Mathematical and Computational Sciences

---

## 📸 Sample Results

| Input (Degraded) | CNN Output (Enhanced) | Reference (Clean) |
|---|---|---|
| ![degraded](assets/degraded.png) | ![output](assets/output.png) | ![reference](assets/reference.png) |

---

## 🎯 Problem Statement

Underwater images suffer from severe degradation due to light absorption and scattering:

- 🔴 **Red channel** disappears first (below 3m)
- 🟠 **Orange/Yellow** disappears next (below 5m)
- 🔵 **Blue dominates** — images look hazy and color-distorted

Our CNN model learns to **restore lost colors** and improve overall image quality.

---

## 🏗️ Model Architecture

### Simple CNN (Current Implementation)

```
Input Image (3 × 256 × 256)
        ↓
Conv2d(3 → 32)  + ReLU
        ↓
Conv2d(32 → 64) + ReLU
        ↓
Conv2d(64 → 64) + ReLU
        ↓
Conv2d(64 → 32) + ReLU
        ↓
Conv2d(32 → 3)  + Sigmoid
        ↓
Output Image (3 × 256 × 256)
```

**Total Parameters:** 75,651

---

## 📊 Results

| Model | PSNR (dB) | Dataset |
|---|---|---|
| Simple CNN (Ours) | 16.98 | UIEB (50 pairs) |

> 🔧 Work in Progress — U-Net with Color Attention Module coming next!

---

## 📦 Dataset — UIEB (Underwater Image Enhancement Benchmark)

| Detail | Info |
|---|---|
| Total Images | 890 real underwater images |
| Paired | Yes — each image has a clean reference image |
| Used for training | 50 matched pairs (40 train / 10 val) |

### Download Links

- 📥 **Raw Underwater Images (raw-890):**
  [Google Drive](https://drive.google.com/drive/folders/1y5eUY-tg7mbUtZwAZcS57TbMhsfMch0V)

- 📥 **Reference Clean Images (reference-890):**
  [Google Drive](https://drive.google.com/file/d/1cA-8CzajnVEL4feBRKdBxjEe6hwql6Z7/view?usp=drivesdk)

- 📄 **Original Paper:**
  [An Underwater Image Enhancement Benchmark Dataset and Beyond (IEEE TIP 2019)](https://ieeexplore.ieee.org/document/8917818)

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/rathod24-code/UIE-Project.git
cd UIE-Project
```

### 2. Install Dependencies
```bash
pip install torch torchvision
pip install opencv-python
pip install scikit-image
pip install matplotlib numpy
```

### 3. Run on Google Colab (Recommended)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com)

- Open `UIE_CNN.ipynb` in Google Colab
- Enable GPU: Runtime → Change runtime type → **T4 GPU**
- Mount Google Drive and set dataset paths
- Run all cells!

---

## 💻 Project Structure

```
UIE-Project/
├── UIE_CNN.ipynb       ← Main training notebook (Google Colab)
├── assets/             ← Sample result images for README
│   ├── degraded.png
│   ├── output.png
│   └── reference.png
└── README.md
```

---

## 🔧 Key Concepts

| Concept | Description |
|---|---|
| **CNN** | Learns to extract and restore image features |
| **MSE Loss** | Measures pixel-level difference between output and reference |
| **PSNR** | Peak Signal-to-Noise Ratio — image quality metric (higher = better) |
| **SSIM** | Structural Similarity Index (closer to 1 = better) |

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0-orange)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green)
![Colab](https://img.shields.io/badge/Google_Colab-T4_GPU-yellow)

---

## 🗺️ Roadmap

- [x] Simple CNN baseline
- [x] Train on UIEB dataset  
- [x] Evaluate PSNR score
- [ ] U-Net with Color Attention Module
- [ ] Train on full 890 image pairs
- [ ] Compare with state-of-the-art methods

---

## 🙏 Acknowledgements

- **Dr. Jidesh P.**, NIT Karnataka — Research Supervisor
- **Neeraj Krishnan P.K.**, MACS NITK — Lab Mentor
- UIEB Dataset — Li et al., IEEE TIP 2019

---

## 📄 References

1. Li, C. et al. "An Underwater Image Enhancement Benchmark Dataset and Beyond." IEEE TIP, 2019.
2. Ronneberger et al. "U-Net: Convolutional Networks for Biomedical Imag
