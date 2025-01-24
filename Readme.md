# Real-Time Sign Language Detector using YOLOv8

This project implements a **real-time sign language detector** using the **YOLOv8 architecture**. The system detects and classifies hand signs from live video feeds or pre-recorded videos, making it a valuable tool for improving communication accessibility.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Dependencies](#dependencies)
4. [Usage Instructions](#usage-instructions)
   - [Training the Model](#training-the-model)
   - [Running Real-Time Detection](#running-real-time-detection)
5. [Results](#results)
6. [Implementation Details](#implementation-details)
7. [File Structure](#file-structure)
8. [Acknowledgements](#acknowledgements)

---

## Project Overview

This project leverages **YOLOv8** for real-time detection and classification of sign language gestures. Key highlights include:
- Custom training on a labeled dataset of sign language gestures.
- Real-time detection capabilities using a webcam or video input.
- Optimized performance for accuracy and speed.

---

## Features

- Implements **YOLOv8** for efficient object detection.
- Real-time detection and classification of sign language gestures.
- Works with live webcam feeds or video files.
- Includes visualization of bounding boxes and class labels on detected signs.
- Scalable for additional sign classes with retraining.

---

## Dependencies

Ensure the following Python packages are installed:
- `ultralytics` (YOLOv8 framework)
- `opencv-python`
- `numpy`
- `torch`

Install them using pip:
```bash
pip install ultralytics opencv-python numpy torch
```

---

## Usage Instructions

### Training the Model
To train the YOLOv8 model on a custom dataset:
```bash
python sign_language_detector.py train --data <path_to_data.yaml> --epochs <num_epochs>
```

### Running Real-Time Detection
To run the detector in real time:
```bash
python sign_language_detector.py detect --source <webcam_or_video_path>
```
- Replace `<webcam_or_video_path>` with `0` for the webcam or a file path for a video.

---

## Results

- The model achieves high detection accuracy on sign language gestures, with real-time inference at 30+ FPS.
- Bounding boxes and class labels are accurately displayed on detected signs.

---

## Implementation Details

1. **Model Architecture**:
   - Based on YOLOv8, optimized for real-time performance.
2. **Dataset**:
   - Custom dataset with labeled sign language gestures.
   - Data augmentation applied to enhance model robustness.
3. **Optimization**:
   - Loss function: Multi-class object detection loss.
   - Optimizer: Adam with learning rate scheduling.
4. **Inference**:
   - Utilizes OpenCV for real-time video feed processing.

---

## File Structure

```
.
├── sign_language_detector.py  # Main script for training and detection
├── data/                      # Directory for training data and annotations
├── models/                    # Directory for saving trained models
├── results/                   # Directory for storing detection outputs
└── README.md                  # This file
```

---

## Acknowledgements

This project utilizes the **YOLOv8 framework by Ultralytics** for efficient object detection. Special thanks to open-source contributors and dataset providers for enabling this work.
