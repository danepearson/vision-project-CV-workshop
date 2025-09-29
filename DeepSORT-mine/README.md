## This folder is for running the YOLOv8 detection and DeepSORT tracking models.

### About YOLOv8:
- YOLO (You Only Look Once) is a real-time object detection algorithm that uses a deep learning approach (passes images through a Neural Network only once... hence "YOLO") to process images
- Its single-pass approach enables real-time detection which makes it great for applications like self-driving cars and video surveillance
- YOLO maintains high accuracy in detecting and classifying objects. It simultaneously predicts bounding boxes and class probabilities, contributing to fewer false positives

### About DeepSORT:
- DeepSORT is a multi-object tracking algorithm
- It builds upon the Simple Online and Realtime Tracking (SORT) algorithm by integrating deep learning to enhance tracking robustness
- DeepSORT can continue to track an object or objects even after they were occluded (hidden or obstructed) or its identity switched
- Using a Kalman filter, it can predict the future location and state of a tracked object. This helps maintain the object's identity and location even when it is temporarily hidden from view due to occlusion
- Using a Convolutional Neural Network (CNN), it also extracts appearance features from the detected objects. These features act as a "visual fingerprint" for each object and allows for re-identification after occlusion or identity changes

#### YOLO and DeepSORT are often used in conjunction for tasks that require both detection and tracking in real-time
***
### How do I run this?
#### First run `python3 object_detection.py` and watch the program run on the video
#### Then run `python3 object_detection_tracking.py` and see how the tracking performs, especially when there is occlusion!
