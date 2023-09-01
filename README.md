# Highway Vehicle Detection using OpenCV

This project uses OpenCV and the TensorFlow Object Detection API to detect and track vehicles on the highway. It also estimates the speed and the distance of the vehicles from the camera.

## Motivation

The motivation behind this project is to create a system that can monitor the traffic conditions on the highway and provide useful information such as the number of vehicles, their speeds, and their positions. This information can be used for various purposes such as traffic management, safety analysis, or law enforcement.

## Methodology

The project consists of two main components: vehicle detection and vehicle tracking.

### Vehicle Detection

The vehicle detection component uses a pre-trained MobileNet SSD model from the TensorFlow Object Detection API to detect vehicles in each frame of the video. The model is optimized for speed and accuracy, and can detect various types of vehicles such as cars, trucks, buses, or motorcycles. The model outputs a list of bounding boxes and confidence scores for each detected vehicle.

### Vehicle Tracking

The vehicle tracking component uses the OpenCV library to track the detected vehicles across multiple frames. It uses the CamShift algorithm to adaptively adjust the size and orientation of the bounding boxes based on the color histogram of the vehicle. It also assigns a unique ID to each tracked vehicle and maintains a history of its position and speed.

## Results

The project can successfully detect and track vehicles on the highway and estimate their speed and distance from the camera. The results are displayed on a graphical user interface (GUI) that shows the original video, the detected bounding boxes, and the speed and distance measurements. The results are also stored in a CSV file that contains the frame number, vehicle ID, bounding box coordinates, speed, and distance for each tracked vehicle.

## Requirements

To run this project, you will need:

- Python 3.7 or higher
- OpenCV 4.5 or higher
- TensorFlow 2.4 or higher
- TensorFlow Object Detection API
- Numpy
- Pandas
- Matplotlib
- PyQt5

## References

This project is based on the following sources:

- [OpenCV Vehicle Detection, Tracking, and Speed Estimation](^3^) by Adrian Rosebrock
- [Video road vehicle detection and tracking based on OpenCV](^4^) by Liang Zhang et al.
- [Lane And Vehicle Detection](^5^) by Justin Heaton
