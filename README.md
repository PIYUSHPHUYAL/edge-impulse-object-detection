# Object Detection using ESP32-CAM and Edge Impulse

This project demonstrates how to build an image recognition system using the ESP32-CAM module and the Edge Impulse platform. The system identifies vegetables such as potatoes, tomatoes, and onions, and displays the results on an optional OLED screen. This project introduces the concepts of edge computing and object recognition while showcasing the capabilities of ESP32-CAM.

---

## Table of Contents
- [Overview](#overview)
- [What is AI on Edge?](#what-is-ai-on-edge)
- [What is Object Recognition?](#what-is-object-recognition)
- [Features](#features)
- [Components Required](#components-required)
- [Circuit Diagram](#circuit-diagram)
- [Steps to Build](#steps-to-build)
  - [1. Data Acquisition](#1-data-acquisition)
  - [2. Building the ML Model](#2-building-the-ml-model)
  - [3. Testing the Prototype](#3-testing-the-prototype)
- [Software and Tools](#software-and-tools)
- [Results](#results)
- [Future Enhancements](#future-enhancements)
- [Credits](#credits)

---

## Overview
This project utilizes edge computing to process data locally on the ESP32-CAM, avoiding the need for cloud servers. The Edge Impulse platform is used to train a machine learning model, which is then deployed on the ESP32-CAM for real-time vegetable recognition.

---

## What is AI on Edge?
Edge computing allows AI algorithms to run on low-power devices like microcontrollers, enabling faster data processing by eliminating the need for remote servers. This project applies edge computing for real-time object detection.

---

## What is Object Recognition?
Object recognition refers to identifying and labeling objects within images or videos. In this project, the ESP32-CAM recognizes three types of vegetables (potatoes, tomatoes, and onions) by analyzing their features.

---

## Features
- Real-time vegetable detection
- Compact and cost-effective solution using ESP32-CAM
- Easy deployment via Edge Impulse
- Optional OLED display for visual feedback

---

## Components Required
- **ESP32-CAM** x1  
- **USB to Serial Converter** x1  
- **0.96” OLED Display** (optional) x1  
- **Breadboard** x1  
- **Jumper wires** (as needed)  
- **Vegetables** (potatoes, tomatoes, onions)  

### Software Tools
- [Edge Impulse](https://www.edgeimpulse.com) for training the model
- [Arduino IDE](https://www.arduino.cc/en/software) for programming the ESP32-CAM

---

## Circuit Diagram
Connect the ESP32-CAM to the USB to Serial Converter for programming. If using an OLED display, connect it to the I2C pins of the ESP32-CAM. Refer to the detailed circuit diagram in the "Images" folder.

---

## Steps to Build

### 1. Data Acquisition
- **Option 1**: Download datasets from platforms like Kaggle or OpenML.  
- **Option 2**: Collect images manually using a phone or camera.  
- **Option 3**: Use the ESP32-CAM to capture images directly (recommended).  

### 2. Building the ML Model
1. Sign up on [Edge Impulse](https://www.edgeimpulse.com).
2. Create a new project and upload the collected dataset.
3. Preprocess the images (resize to 256x256px) and extract features.
4. Train a Convolutional Neural Network (CNN) model.

### 3. Testing the Prototype
- Deploy the trained model onto the ESP32-CAM.
- Use the serial monitor or OLED display to view detection results.

---

## Results
The ESP32-CAM successfully detects and identifies vegetables, displaying the results on the OLED or serial monitor. This showcases the feasibility of deploying AI on low-power devices.

---

## Future Enhancements
- Expand the dataset to include more vegetables or other objects.
- Improve model accuracy by using a larger and more diverse dataset.
- Implement advanced visualization techniques for better user interaction.

---

## Credits
This project was inspired by tutorials from [Circuit Digest](https://circuitdigest.com). The Edge Impulse platform and EloquentEsp32cam library were essential for successful implementation.

---
