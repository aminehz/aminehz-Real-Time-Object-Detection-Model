# Real-Time Object Detection using YOLOv8

This project demonstrates real-time object detection using the YOLOv8 (You Only Look Once) model. The implementation captures video from a webcam and processes each frame to detect objects, displaying the bounding boxes and class names.

## Overview

The goal of this project is to use the YOLOv8 model to perform real-time object detection on a video feed from a webcam. The detected objects are displayed with bounding boxes and class names.

## Project Structure

- `real_time_object_detection.py`: The main script that captures video from the webcam, processes each frame using YOLOv8, and displays the results.
- `yolo-Weights/yolov8n.pt`: The pre-trained YOLOv8 model weights.

## Model Description

The model used in this project is the YOLOv8 model from Ultralytics. YOLOv8 is a state-of-the-art, real-time object detection model that can detect a wide range of objects with high accuracy.

1. **Device Setup**:
   - The model checks if CUDA (GPU) is available and sets the device accordingly to ensure efficient processing.

2. **Webcam Initialization**:
   - The script initializes the webcam with a resolution of 640x480 for capturing video frames.

3. **Model Loading**:
   - The pre-trained YOLOv8 model weights are loaded and moved to the specified device (CPU or GPU).

4. **Object Detection**:
   - For each frame captured from the webcam, the model performs object detection and retrieves the bounding boxes, class names, and confidence scores.
   - Bounding boxes and class names are drawn on the frames.

