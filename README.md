# ANN2DL Challenge 2 - Image Classification

This repository contains the scripts and final report for Challenge 2 (Image Classification) of the Artificial Neural Networks and Deep Learning course at Politecnico di Milano, Academic Year 2025/2026.

## 📋 Overview

This challenge focused on developing deep learning models for image classification using transfer learning and fine-tuning techniques. The repository includes multiple experimental approaches, data preprocessing scripts, and a comprehensive report documenting our methodology and results.

## 📁 Repository Structure

```
ANN2DL_ch2/
├── README.md                          # This file
├── report_ch2.pdf                     # Final report with methodology and results
└── scripts/                           # All implementation scripts
    ├── README.md                      # Detailed scripts documentation
    ├── Patches_extractor.ipynb        # Preprocessing: patch extraction utility
    └── [Model notebooks]              # Various architectures and techniques
```

## 📄 Report

The file `report_ch2.pdf` contains our comprehensive analysis including:
- Problem statement and dataset description
- Methodology and experimental setup
- Architecture comparisons and ablation studies
- Data augmentation strategies
- Transfer learning and fine-tuning approaches
- Results and performance metrics
- Conclusions and future work

## 🚀 Scripts

All scripts are located in the `/scripts` directory and are implemented as Jupyter notebooks. Each notebook is self-contained and runnable with a dataset folder named `clean_patches`.

### Architecture Implementations

The repository includes implementations using the following architectures, all with Transfer Learning (TL) and Fine-Tuning (FT):

#### Standard Architectures
- **VGG16_TL_FT.ipynb** - VGG16 architecture
- **ResNet50_GAP_TL_FT.ipynb** - ResNet50 with Global Average Pooling
- **ResNet152_TL_FT.ipynb** - Deeper ResNet152 variant
- **DENSENet121_TL_FT.ipynb** - DenseNet121 architecture
- **Xception_TL_FT.ipynb** - Xception architecture
- **EfficientNetB2_TL_FT.ipynb** - EfficientNetB2 architecture
- **ConvNextSmall_TL_FT.ipynb** - ConvNeXt Small architecture
- **MobileNet_TL_FT_PATCHES.ipynb** - MobileNet optimized for patches

#### Medical Imaging Specific
- **KIMIANET_TL_FT.ipynb** - KimiaNet (specialized for histopathology images)

#### Data Augmentation Experiments
- **MixUp_GAP_ResNet50_TL_FT.ipynb** - ResNet50 with MixUp augmentation
- **Flip+MixUp_ResNet50_TL_FT.ipynb** - ResNet50 with Flip and MixUp
- **Bn+Flip+MixUp_ResNet50_TL_FT.ipynb** - ResNet50 with Batch Normalization, Flip, and MixUp

#### Baseline and Preprocessing
- **Baseline_patches.ipynb** - Baseline model for patch-based classification
- **Patches_extractor.ipynb** - Utility to extract patches from full-resolution images

### Script Naming Convention

Scripts follow the naming pattern: `[Augmentation+]Architecture_TL_FT.ipynb`
- **Augmentation**: Data augmentation techniques used (e.g., MixUp, Flip, Bn)
- **Architecture**: Neural network architecture (e.g., ResNet50, VGG16)
- **TL**: Transfer Learning
- **FT**: Fine-Tuning

## 🔧 Usage

### Prerequisites
- Python 3.x
- Jupyter Notebook/Lab
- TensorFlow/Keras or PyTorch (depending on notebook)
- Standard deep learning libraries (NumPy, Pandas, Matplotlib, etc.)

### Running the Scripts

1. **Prepare your dataset**: Create a folder named `clean_patches` with your image dataset
2. **Open a notebook**: Choose any script from the `/scripts` directory
3. **Run all cells**: Execute the notebook cells sequentially

```bash
jupyter notebook scripts/ResNet50_GAP_TL_FT.ipynb
```

### Extracting Patches

To preprocess full-resolution images into patches:

```bash
jupyter notebook scripts/Patches_extractor.ipynb
```

## 🎯 Key Techniques

- **Transfer Learning**: Leveraging pre-trained weights from ImageNet
- **Fine-Tuning**: Adapting pre-trained models to the specific classification task
- **Data Augmentation**: MixUp, horizontal/vertical flips, batch normalization
- **Patch-Based Training**: Processing high-resolution images via patch extraction
- **Global Average Pooling**: Reducing spatial dimensions while preserving features

## 📊 Results

Detailed results, metrics, and comparative analysis are available in the `report_ch2.pdf` file. The report includes:
- Accuracy and loss curves
- Confusion matrices
- Per-class performance metrics
- Architecture comparison tables
- Ablation study results

## 👥 Authors

Alessandro De Matteis and team - Politecnico di Milano

## 📅 Academic Year

2025/2026

## 📧 Contact

For questions or collaboration opportunities, please contact through the repository issues or Politecnico di Milano channels.

---

*This project was developed as part of the Artificial Neural Networks and Deep Learning course at Politecnico di Milano.*
