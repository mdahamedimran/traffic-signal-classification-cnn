# Traffic Signal Classification Using CNN

## Project Overview

This research investigates traffic signal classification using
Convolutional Neural Networks (CNNs) on the LISA Traffic Light
Dataset. Five CNN configurations are evaluated to compare
classification performance and computational efficiency.

## Dataset

- Dataset: LISA Traffic Light Dataset
- Total Samples: 12,000
- Training Samples: 8,400 (70%)
- Validation Samples: 1,800 (15%)
- Testing Samples: 1,800 (15%)
- Image Resolution: 64 × 64 × 3
- Classes: Red, Yellow, Green

[Dataset Source](https://www.kaggle.com/datasets/mbornoe/lisa-traffic-light-dataset)

## CNN Experiments

| ID | Model | Parameters | Validation Accuracy |
|---|---|---:|---:|
| EXP01 | Baseline CNN | 1,142,339 | 100% |
| EXP02 | CNN + Data Augmentation | 1,142,339 | 100% |
| EXP03 | CNN + Class Weighting | 1,142,339 | 100% |
| EXP04 | CNN + Augmentation + Class Weighting | 1,142,339 | 100% |
| EXP05 | Lightweight CNN | 110,147 | 99.94% |

## Key Findings

- Four CNN configurations achieved 100% validation accuracy.
- The lightweight CNN achieved 99.94% validation accuracy.
- The lightweight model reduced trainable and non-trainable
  parameters combined by approximately 90.36%.
- Sequence-based dataset splitting was used to reduce data leakage.
- Independent test evaluation is pending.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- OpenCV
- Matplotlib
- Seaborn
- Scikit-learn
- Kaggle GPU Environment

## Repository Structure

```text
traffic-signal-classification-cnn/
├── dataset/
├── paper/
├── research_outputs/
├── saved_models/
├── .gitignore
├── README.md
├── requirements.txt
└── traffic-signal-classification.ipynb
```

## Research Objectives

- Develop a CNN-based traffic signal classification system.
- Investigate the effects of data augmentation.
- Evaluate the impact of class weighting.
- Compare classification performance across five models.
- Develop a computationally efficient lightweight CNN.

## Research Status

- [x] Dataset collection
- [x] Data preprocessing
- [x] Dataset splitting and leakage checks
- [x] CNN model development
- [x] Training and validation
- [x] Model comparison
- [x] Computational efficiency analysis
- [ ] Independent test evaluation
- [ ] Final research paper

## Research Paper

The research paper will be uploaded to the `paper/` directory
after the final evaluation is completed.
