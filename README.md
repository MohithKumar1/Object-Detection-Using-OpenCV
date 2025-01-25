# Object-Detection-Using-OpenCV

This repository contains a Python script for object detection using the OpenCV DNN module. The code utilizes the SSD MobileNet V3 model trained on the COCO dataset to detect and classify objects in an image.

# Requirements
Before running the code, ensure you have the following installed:

Python 3.6+
OpenCV (cv2)
Matplotlib
NumPy

# Files in This Repository

ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt: The configuration file for the model.
frozen_inference_graph.pb: The pre-trained model's frozen graph.
labels.txt: A text file containing the class labels for the COCO dataset.
boy.jpg: A sample image to test the object detection.
object_detection.py: The main Python script for running object detection.

# Code Explanation

Load the Model and Class Labels:
The cv2.dnn_DetectionModel is initialized with the configuration and model files.
The class labels are read from the labels.txt file.

Image Preprocessing:
Input image is resized, scaled, mean-subtracted, and converted to RGB format.

Object Detection:
The model.detect() method identifies objects in the image based on a confidence threshold.

Visualization:
Bounding boxes and class labels are drawn on the detected objects using OpenCV functions.

# Output
After running the script, a visualized image will be displayed with bounding boxes and class labels for detected objects. The detection results will also be printed to the console.
