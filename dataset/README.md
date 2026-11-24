# Dataset Documentation

## Dataset Source

LISA Traffic Light Dataset

https://www.kaggle.com/datasets/mbornoe/lisa-traffic-light-dataset

## Dataset Summary

| Property | Value |
|---|---|
| Total Samples | 12,000 |
| Training Samples | 8,400 |
| Validation Samples | 1,800 |
| Testing Samples | 1,800 |
| Image Size | 64 × 64 pixels |
| Color Format | RGB |
| Number of Classes | 3 |

## Class Labels

- 0: Red
- 1: Yellow
- 2: Green

## Preprocessing

- Traffic light bounding box extraction
- Image resizing with aspect-ratio-preserving padding
- RGB color conversion
- Pixel normalization
- Sequence-based dataset splitting
- Duplicate and data leakage checks

## Preprocessed Dataset Structure

- X_train.npy
- X_val.npy
- X_test.npy
- y_train.npy
- y_val.npy
- y_test.npy
- dataset_metadata.csv

## Dataset Availability

The dataset files are not included in this repository.
Download the original dataset from the source provided
above and follow the preprocessing steps in the research
notebook.

Refer to the original dataset's licensing terms before
using or redistributing the images.
