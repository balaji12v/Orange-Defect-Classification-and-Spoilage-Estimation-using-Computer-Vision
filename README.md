# Orange Defect Classification and Spoilage Estimation using Computer Vision

## Project Overview

This project focuses on building a Computer Vision pipeline to detect and classify orange defects and estimate fruit spoilage percentage. Two different approaches were implemented and compared:

1. Classical Computer Vision + Machine Learning
2. Deep Learning using Transfer Learning

The system classifies oranges into:

- Fresh
- Blackspot
- Canker
- Greening

Additionally, a spoilage estimation module was developed to calculate the percentage of damaged fruit area.

---

## Features

- Orange defect classification
- Classical Computer Vision pipeline using HSV + LBP features
- Random Forest classifier implementation
- MobileNetV2 transfer learning model
- Spoilage percentage estimation using image segmentation
- Model comparison and evaluation
- Confusion matrix and classification metrics analysis

---

## Approaches Implemented

### Approach 1: Classical Computer Vision + Random Forest

Pipeline:

Image → Resize → HSV Feature Extraction → LBP Texture Features → Random Forest → Prediction

Performance:

- Accuracy: 95.98%

---

### Approach 2: MobileNetV2 Transfer Learning

Pipeline:

Image → Resize → Normalization → MobileNetV2 → Dense Layers → Prediction

Performance:

- Test Accuracy: 93.94%

---

## Spoilage Estimation

Spoilage percentage was calculated using image segmentation techniques.

Formula:

Spoilage Percentage =

(Defect Pixels / Fruit Pixels) × 100

Example results:

| Disease Type | Spoilage Percentage |
|---------------|---------------------|
| Blackspot | 9.47% |
| Canker | 72.33% |
| Greening | 3.28% |

---

## Dataset Information

Dataset contains orange images belonging to:

- Fresh
- Blackspot
- Canker
- Greening

Total Images: 1090

Train Images: 991

Test Images: 99

**Note:** Dataset has not been included in this repository due to size limitations.

---

## Tech Stack

- Python
- OpenCV
- Scikit-Learn
- TensorFlow
- MobileNetV2
- NumPy
- Matplotlib
- Computer Vision
- Machine Learning

---

## Project Structure

```

project/

├── dataset/

├── eda/

├── preprocessing/

├── model1/
│ ├── random_forest_model.pkl

├── model2/
│ ├── mobilenetv2_model.keras

├── example_run.ipynb

├── requirements.txt

└── README.md

```

---

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

---

## Future Improvements

- Larger dataset collection
- Improved spoilage segmentation
- Additional disease categories
- Real-time deployment
- Object detection based localization

---

## Author

Balaji
