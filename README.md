Indian Sign Language Translator

Computer Vision & Deep Learning Project

June 2025

Overview

Indian Sign Language (ISL) is an important medium of communication for individuals with hearing and speech impairments. This project focuses on developing a near real-time Indian Sign Language Translator capable of recognizing hand gestures from live webcam input using Computer Vision and Deep Learning techniques.

The system combines face detection, hand detection, image preprocessing, and gesture classification to improve recognition accuracy under varying backgrounds and lighting conditions.

Background

Traditional sign language recognition systems often struggle with changing lighting conditions, background clutter, and inconsistent hand positioning. This project addresses these challenges by integrating multiple Computer Vision techniques before performing gesture classification.

The implementation utilizes a pre-trained hand detection model along with image preprocessing and Transfer Learning to recognize Indian Sign Language gestures efficiently.

Note: This project is intended for learning and experimentation with Computer Vision and Deep Learning techniques. The current implementation focuses on building a functional recognition pipeline while leaving room for future improvements.

Objectives

The project aims to:

• Develop a near real-time Indian Sign Language recognition system.

• Detect hands accurately from live webcam input.

• Minimize the effects of varying backgrounds and illumination.

• Classify Indian Sign Language gestures using a deep learning model.

Dataset

Dataset: Indian Sign Language Dataset

Classes: 10 Gesture Classes

Images per Class: Approximately 2,300+

Image Type: RGB Images

The dataset is preprocessed before training using image enhancement and segmentation techniques to improve recognition performance.

Key Features

• Near real-time gesture recognition

• Face-based activation mechanism

• YOLOv3-based hand detection

• Skin segmentation using HSV and YCbCr color spaces

• Transfer Learning with SqueezeNet

• Background and illumination robustness

Project Workflow
Detect the user's face using OpenCV Haar Cascade.
Activate the recognition pipeline after consecutive face detections.
Detect hand regions using a pre-trained YOLOv3 model.
Crop and preprocess the detected hand.
Apply skin segmentation to reduce background noise.
Pass the processed image to the trained SqueezeNet model.
Predict the corresponding Indian Sign Language gesture.
Technologies Used

• Python

• TensorFlow

• Keras

• OpenCV

• YOLOv3

• ImageAI

• NumPy

• Pillow

Project Structure

Indian-Sign-Language-Translator/
--- app/ # Main application

--- dataset/ # Dataset preparation scripts

--- preprocessing/ # Image preprocessing modules

--- model/ # Model training notebooks

--- requirements.txt

--- README.md

Requirements

Python 3.8 or higher

Jupyter Notebook (Optional)

TensorFlow

OpenCV

ImageAI

NumPy

Pillow

All required dependencies are listed in requirements.txt.

To install the dependencies:

pip install -r requirements.txt

Running the Project
Environment Setup

It is recommended to create a virtual environment before installing the dependencies.

Install all required packages using:

pip install -r requirements.txt

Launch the Application

Run the main application:

python main.py

Once the webcam starts, the application detects the user's face and automatically begins recognizing hand gestures.

Future Improvements

• Support additional Indian Sign Language gestures.

• Improve model accuracy through hyperparameter tuning.

• Replace Haar Cascade with more robust face detection models.

• Deploy the application as a desktop or web-based solution.

• Optimize inference speed for smoother real-time performance.

Notes

This project demonstrates the practical application of Computer Vision and Deep Learning techniques for real-time gesture recognition. It integrates object detection, image preprocessing, transfer learning, and classification into a complete recognition pipeline while providing a foundation for future enhancements in sign language translation.
