# Vehicle Detection, Tracking, and Speed Estimation

This repository contains Python scripts for detecting, tracking, and estimating the speed of vehicles in a video using YOLOv8 and OpenCV. The project is divided into four main scripts, each focusing on a specific aspect of vehicle detection and analysis.

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Requirements](#requirements)
4. [Usage](#usage)
5. [Script Details](#script-details)


## Introduction
This project leverages the YOLOv8 model for object detection and OpenCV for video processing. It includes functionalities for detecting vehicles, tracking their movements, and estimating their speeds. The scripts are designed to work with video files and can be adapted for real-time applications.

## Features
- **Vehicle Detection**: Detects cars, buses, and trucks using YOLOv8.
- **Vehicle Tracking**: Tracks vehicles across frames using a custom tracker.
- **Speed Estimation**: Estimates the speed of detected vehicles.
- **Distance Estimation**: Calculates the distance of vehicles from the camera using the pinhole camera model.
- **Visualization**: Displays bounding boxes, IDs, and speed information on the video frames.

## Requirements
- Python 3.8 or higher
- OpenCV (`cv2`)
- Pandas (`pandas`)
- NumPy (`numpy`)
- Ultralytics (`ultralytics`)
- cvzone (`cvzone`)


## Script Details

### 1. `Detection and Tracking Code`
- **Description**: Detects and tracks vehicles (cars, buses, trucks) in a video.
- **Features**:
  - Uses YOLOv8 for object detection.
  - Tracks vehicles using a custom tracker.
  - Displays bounding boxes and IDs on the video frames.
  - Draws neon lines to show the path of tracked vehicles.

### 2. `Vehicle Distance Estimator`
- **Description**: Estimates the distance of detected vehicles from the camera.
- **Features**:
  - Uses the pinhole camera model for distance estimation.
  - Displays the estimated distance on the video frames.
  - Works for cars, buses, and trucks.

### 3. `Speed Estimation Code`
- **Description**: Estimates the speed of detected vehicles.
- **Features**:
  - Uses a custom algorithm to calculate speed based on vehicle movement.
  - Displays the estimated speed on the video frames.
  - Handles stationary vehicles and smooths speed estimates.

### 4. `Tracker_module.py`
- **Description**: Contains the custom tracker class used in the above scripts.
- **Features**:
  - Tracks objects based on their center points.
  - Assigns unique IDs to detected objects.
  - Cleans up unused IDs to optimize performance.


---

This README provides an overview of the project and the scripts. 
