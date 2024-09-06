# Obstacle Avoidance for Autonomous Bot

This repository contains a basic algorithm for detecting obstacles using OpenCV and guiding an autonomous bot to avoid them. 
The code captures video from the camera, processes the frames to identify obstacles, and provides directional commands to navigate around these obstacles.

## Overview

The algorithm uses a video feed from a camera (e.g., a webcam) and processes each frame to detect potential obstacles. 
It uses contour detection to identify objects and determines the movement direction based on the location of these obstacles within the frame. 
The bot can move forward, turn left, right, or reverse based on the position of obstacles detected.

## Features

- **Obstacle Detection**: Detects obstacles in real-time using contour analysis.
- **Movement Commands**: Provides directional commands (`forward`, `left`, `right`, `reverse`) to avoid obstacles.
- **Visual Feedback**: Displays the video feed with detected obstacles highlighted by bounding boxes and labels.

## Limitations

- **Color Sensitivity**: The algorithm struggles to detect obstacles that are white or similar to white, as they are often not identified efficiently by the thresholding process used in the detection pipeline.
- **Simple Directional Commands**: The movement commands are basic and may need further tuning for specific applications, especially in complex environments.


