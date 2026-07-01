# Object Detection Evaluation Pipeline

This project implements a complete object detection evaluation pipeline from scratch using only NumPy and Pandas. No external detection libraries (torchvision, ultralytics, detectron2) are used.

## What This Project Does

The pipeline evaluates object detection model performance by comparing predicted bounding boxes against ground truth annotations using standard metrics:

- **IoU (Intersection over Union):** Measures overlap between predicted and ground truth boxes
- **NMS (Non-Maximum Suppression):** Removes duplicate detections of the same object
- **Precision & Recall:** Quantifies detection accuracy and completeness
- **Average Precision (AP@0.5):** Summarizes performance across all confidence thresholds
- **PR Curve:** Visualizes the precision-recall trade-off

## Key Results

- Ground Truth Objects: 8
- Predicted Boxes: 12
- Detections after NMS: 10
- Precision: 30.00%
- Recall: 37.50%
- Average Precision (AP@0.5): 47.92%

## Files Included

- `object_detection_evaluation.ipynb` - Main Jupyter Notebook with all implementations
- `ground_truth_boxes.csv` - Ground truth bounding box annotations
- `predicted_boxes.csv` - Model predictions with confidence scores
- `precision_recall_curve.png` - PR curve visualization output

## Requirements

- Python 3.7+
- NumPy
- Pandas
- Matplotlib
- SciPy (for trapezoidal integration)

## How to Run

1. Clone this repository
2. Install dependencies: `pip install numpy pandas matplotlib scipy`
3. Open and run the Jupyter Notebook
4. All results will be printed and the PR curve will be saved

## Academic Context

This was created as part of a Computer Vision course practical on object detection evaluation methodologies.
