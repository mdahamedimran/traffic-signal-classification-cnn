# Traffic Signal Classification Using CNN

## Project Overview

This research investigates traffic signal classification
using Convolutional Neural Networks (CNNs) on the LISA
Traffic Light Dataset. Five CNN configurations are
compared in terms of classification performance,
generalization and parameter efficiency.

## Dataset

- Dataset: LISA Traffic Light Dataset
- Total Samples: 12,000
- Training Samples: 8,400 (70%)
- Validation Samples: 1,800 (15%)
- Independent Test Samples: 1,800 (15%)
- Image Resolution: 64 × 64 × 3
- Classes: Red, Yellow and Green

[Dataset Source](https://www.kaggle.com/datasets/mbornoe/lisa-traffic-light-dataset)

## Experimental Results

| Model | Validation Accuracy | Test Accuracy | Macro F1 | Parameters |
|---|---:|---:|---:|---:|
| EXP01 - Baseline | 100% | 97.06% | 86.48% | 1,142,339 |
| EXP02 - Augmented | 100% | 96.50% | 85.13% | 1,142,339 |
| EXP03 - Weighted | 100% | 98.89% | 93.90% | 1,142,339 |
| EXP04 - Combined | 100% | 98.50% | 91.80% | 1,142,339 |
| EXP05 - Lightweight | 99.94% | 98.22% | 94.48% | 110,147 |

## Key Findings

- EXP03 achieved the highest independent test accuracy
  of 98.89%.
- EXP05 achieved the highest macro F1-score of 94.48%.
- EXP05 achieved a macro recall of 98.75%.
- EXP05 correctly classified all 50 actual Yellow
  test samples.
- The lightweight CNN reduced model parameters by 90.36%.
- Class weighting improved independent test performance
  compared with the baseline CNN.
- Sequence-based splitting and exact duplicate checks
  were performed to reduce data leakage.

## Methodology

1. Dataset collection and annotation filtering
2. Traffic light bounding box extraction
3. Image resizing and normalization
4. Sequence-based dataset splitting
5. CNN architecture development
6. Data augmentation and class weighting
7. Model training and validation
8. Independent test evaluation
9. Model performance and efficiency comparison

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
- Kaggle

## Repository Structure

traffic-signal-classification-cnn/
├── dataset/
├── independent_test_results/
├── paper/
├── research_outputs/
├── saved_models/
├── .gitignore
├── README.md
├── requirements.txt
├── independent-test-evaluation.ipynb
└── traffic-signal-classification.ipynb

## Research Limitations

- The evaluation is limited to the LISA dataset.
- The independent test set contains only 50 Yellow samples.
- The models classify cropped traffic light images rather
  than detecting traffic lights in full road scenes.
- Further testing is required before real-world deployment.

## Research Status

- [x] Dataset collection
- [x] Data preprocessing
- [x] Dataset splitting and leakage checks
- [x] CNN development
- [x] Training and validation
- [x] Model comparison
- [x] Computational efficiency analysis
- [x] Independent test evaluation
- [x] Classification reports
- [x] Confusion matrices
- [x] Research figures
- [x] GitHub source code and results
- [ ] Final research paper

## Research Paper

The research paper is currently under preparation and
will be available in the paper directory upon completion.
