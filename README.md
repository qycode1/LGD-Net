# LGD-Net: A Lesion-Guided Dual-Encoder Network with Multi-Stage Feature Fusion for Skin Lesion Segmentation

This repository is the official PyTorch implementation of the paper:  
**"LGD-Net: A Lesion-Guided Dual-Encoder Network with Multi-Stage Feature Fusion for Skin Lesion Segmentation"** (Under Review at *Biomedical Signal Processing and Control*).

---
LGD-Net integrates a dual-encoder architecture (CNN and Swin Transformer) with three collaborative modules:
1. **DAMS**: Detail-Aware Multi-Scale Block for boundary and texture representation enhancement.
2. **LGMF (with LQT)**: Lesion-Guided Multi-Feature Fusion Block with shared lesion queries for complementary cross-branch interaction.
3. **EGA**: Edge-Global Guided Attention Block for decoder feature refinement.

---

## 💻 Environment Setup

The codebase is tested with Python 3.8+, PyTorch 1.12.0+, and CUDA 11.3+.

```bash
# Clone the repository
git clone https://github.com/qycode1/LGD-Net.git
cd LGD-Net

# Create a virtual environment (optional)
conda create -n lgdnet python=3.9 -y
conda activate lgdnet

# Install dependencies
pip install -r requirements.txt
