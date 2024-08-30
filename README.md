# Multi-Camera-Person-Tracking-with-Trajectory

## Introduction

This project demonstrates multi-camera person tracking using YOLOv5 for object detection. It reads frames from two video streams (cameras), performs object detection to identify persons, and tracks their movements within specified boundaries. The code uses OpenCV for video input/output and visualization.

## Requirements

Before running this project, ensure you have the following dependencies installed:

- Python 3.x
- OpenCV (cv2)
- PyTorch
- NumPy
- Ultralytics' YOLOv5

You can install these dependencies using `pip`:

```bash
pip install opencv-python-headless torch numpy yolov5
```
## Project Structure
The project directory structure should look like this:

```
project-root/
    ├── your_script.py
    ├── yolov5/
    │   └── yolov5s.pt
    ├── Project007.mp4
    └── Project004.mp4
```

your_script.py: The Python script containing the tracking code.

yolov5/: A directory containing YOLOv5 model checkpoint.

Project007.mp4 and Project004.mp4: Sample video files from cameras.

## How to Use

Clone or download the project repository to your local machine.

Install the required dependencies mentioned in the Requirements section.

Place the YOLOv5 model checkpoint file (yolov5s.pt) in the yolov5/ directory.

Update the boundary coordinates in the script as needed:

## Python boundary code snippet
```
boundary_x1 = 1  # Top-left x-coordinate
boundary_y1 = 1  # Top-left y-coordinate
boundary_x2 = 1280  # Bottom-right x-coordinate
boundary_y2 = 720  # Bottom-right y-coordinate
```

Run the script your_script.py.

The script will open two video streams and display them side by side. It will perform object detection using YOLOv5, track persons, and draw arrows indicating their movement within the specified boundary. The number of persons and their confidence scores are displayed at the bottom of each video stream.

Press 'q' to exit the application.

## Code Explanation

The code uses YOLOv5 to perform object detection on each frame from two cameras, identifying persons.
It keeps track of persons' positions, draws arrows to show their movement direction, and displays confidence scores.
The script visualizes the video streams and boundaries, and it updates the positions of tracked persons in real-time.

## Customization
You can customize this code by adjusting parameters such as boundary coordinates, object classes, and confidence thresholds to suit your specific tracking requirements.

This documentation provides an overview of the multi-camera person tracking project, its requirements, usage instructions, and code documentation. You can further customize and extend this project to suit your specific needs, such as integrating more cameras or using different object detection models.

## Contributors
CH SRICHERAN - sricharan320@gmail.com
PN SANJAY - sanjayperam2604@gmail.com
PVS SUKRITH - sukrithpvs2005@gmail.com
