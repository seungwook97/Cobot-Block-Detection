# Robotic Sorting System with Object Detection and MyCobot Control

## Overview

This project implements a robotic sorting system where blocks move along a conveyor belt. The blocks are detected using the YOLO object detection model and classified as either "normal" or "defective". A MyCobot robotic arm then sorts the blocks into two separate locations based on their classification. The system uses an **Astra U3 depth camera** for precise depth perception and object tracking on the conveyor belt.

## Features

- **Conveyor Belt Simulation**:  
  The blocks move along a conveyor belt, and their movement is tracked for sorting purposes.

- **YOLO Object Detection**:  
  Real-time object detection using the YOLO model to classify blocks as either "True" (normal) or "False" (defective).

- **Robotic Arm Control**:  
  A MyCobot robotic arm sorts the blocks. Normal blocks ("True") are moved to the left, and defective blocks ("False") are moved to the right.

- **Multithreading**:  
  The system uses multithreading to simultaneously detect objects and control the robotic arm for efficient sorting.

- **Astra U3 Depth Camera**:  
  The Astra U3 depth camera provides depth data to detect the blocks and track their movement along the conveyor belt, improving accuracy and reliability.

- **ROS2 Communication**:  
  The system communicates using ROS2 to send the detected object coordinates to the robotic arm for sorting.

## Requirements

- **Python Libraries**:
  - `ultralytics` (for YOLO)
  - `pymycobot` (for MyCobot control)
  - `opencv-python` (for camera and image processing)
  - `threading` (for multithreading)
  - `time` (for delays)
  - `roslibpy` (for ROS2 communication)

  Install required libraries using:
  ```bash
  pip install ultralytics pymycobot opencv-python roslibpy
