# Object Detection with SSD MobileNet V2, LabelImg, and OpenCV

Welcome to the **Image Labeling and Object Detection** repository! This project demonstrates the process of labeling images using the LabelImg tool, applying transfer learning with the *SSD MobileNet V2 FPNLite 320x320* for object detection, and implementing real-time detection using **OpenCV**.

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Image Labeling using LabelImg](#image-labeling-using-labelimg)
- [Object Detection with SSD MobileNet V2](#object-detection-with-ssd-mobilenet-v2)
- [Real-Time Detection using OpenCV](#real-time-detection-using-opencv)
- [Conclusion](#conclusion)

## Introduction

This project showcases a complete workflow for labeling images and training an object detection model using transfer learning. The goal is to create a robust image detection system that can perform real-time detection using OpenCV.

We use the following key components:
- **LabelImg Tool:** For annotating images by creating bounding boxes and labels.
- **SSD MobileNet V2 FPNLite 320x320:** A pre-trained deep learning model for object detection.
- **OpenCV:** For real-time detection using video feeds or webcams.

## Prerequisites

Before starting, make sure you have the following tools and libraries installed:

- **LabelImg:** For labeling the images.
- **TensorFlow:** For training the object detection model.
- **OpenCV:** For real-time image and video processing.
- **Python:** Required for executing scripts.

## Image Labeling using LabelImg

The first step in training an object detection model is to create labeled datasets. LabelImg is a graphical tool used to annotate images by drawing bounding boxes around objects of interest and assigning labels to them.

### Steps to Label Images:
1. Install the **LabelImg** tool and open it.
2. Load the images you want to label.
3. Draw bounding boxes around the objects in the image.
4. Assign appropriate labels to the objects.
5. Save the labeled images in `.xml` format for later use in model training.

## Object Detection with SSD MobileNet V2

Once the images are labeled, we can move on to the next phase: training the object detection model using **SSD MobileNet V2 FPNLite 320x320**.

### Key Concepts:
- **Transfer Learning:** Using a pre-trained model (SSD MobileNet V2) to adapt to a new dataset by fine-tuning.
- **SSD (Single Shot Detector):** A popular object detection architecture that efficiently detects objects in a single forward pass of the network.
- **MobileNet V2:** A lightweight deep learning architecture optimized for mobile devices.

By leveraging transfer learning, we can achieve faster training times and more accurate results, especially when working with small datasets.

## Real-Time Detection using OpenCV

After training the model, we implement real-time object detection using **OpenCV**. OpenCV is an open-source computer vision library that enables efficient real-time image processing and video capture.

### Steps for Real-Time Detection:
1. **Load the Trained Model:** Import the pre-trained SSD MobileNet V2 model into your Python environment using TensorFlow.
2. **Initialize OpenCV:** Use OpenCV to access the webcam or video stream.
3. **Detect Objects:** Pass each frame of the video feed through the model to detect objects in real-time.
4. **Display Results:** Draw bounding boxes around detected objects and display the video with the real-time detection results.

![Screenshot 2024-10-01 212416](https://github.com/user-attachments/assets/289fa372-5da4-4c1b-95e4-145cabbe5137)


This setup allows the detection of objects in real-time, making it suitable for applications like surveillance, monitoring, or any real-time vision-based solutions.



## Conclusion

By combining the **LabelImg** tool for image annotation, the **SSD MobileNet V2 FPNLite 320x320** for transfer learning, and **OpenCV** for real-time object detection, we have built a powerful object detection system. This project demonstrates the complete workflow from labeling images to detecting objects in real-time using a webcam or video stream.

Feel free to explore the repository and experiment with your own datasets and video sources!

---
LabelImg, the popular image annotation tool created by Tzutalin, Thanks!
I would like to thanks Nicholas Renotte, without his Youtube Guidance it wouldn't have been possible to understand the dynamics of object detection and it's working!
