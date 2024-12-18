# Block Detection with Astra Stereo U3 Camera

This project uses the Astra Stereo U3 3D depth camera and ROS2 to detect blocks on a conveyor belt, track their coordinates (x, y, z), and publish the detected coordinates for further processing by a robotic system (e.g., a Cobot).

## Features

- Uses the Astra Stereo U3 3D camera for depth perception.
- Processes infrared (IR) and depth images to detect blocks on a conveyor belt.
- Extracts and publishes the (x, y, z) coordinates of detected blocks.
- Integrates with ROS2 for seamless communication and robot control.

## Requirements

- ROS2 (Humble or higher)
- OpenCV
- cv_bridge
- Astra Stereo U3 Camera

## Installation

### 1. Install ROS2 and dependencies
Follow the instructions for setting up ROS2 on Ubuntu [here](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html).

### 2. Install OpenCV
You can install OpenCV using the following command:

```bash
sudo apt-get install libopencv-dev python3-opencv
