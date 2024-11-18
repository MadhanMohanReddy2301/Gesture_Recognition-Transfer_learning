# Gesture Recognition for Smart TVs

This project implements a deep learning model for gesture recognition, enabling users to control a smart TV without using a remote. The gestures are captured through a webcam and correspond to specific TV commands.

## Table of Contents
- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Project Structure](#project-structure)
- [Models](#models)
  - Conv3D Models
  - CNN + RNN Models
  - Transfer Learning Using MobileNet
- [Results](#results)
- [Conclusion](#conclusion)
- [Usage Instructions](#usage-instructions)

---

## Introduction

This group project aims to develop a deep learning model capable of recognizing five distinct gestures. These gestures are then mapped to TV commands to enhance the user experience.

---

## Problem Statement

The goal is to create a smart TV feature that recognizes five gestures performed by the user, allowing them to control the TV hands-free. The gestures and their corresponding commands are:

- **Thumbs up**: Increase the volume
- **Thumbs down**: Decrease the volume
- **Left swipe**: Jump backward 10 seconds
- **Right swipe**: Jump forward 10 seconds
- **Stop**: Pause the movie

---

## Project Structure

1. **Data Preprocessing**: 
   - Custom video frame extraction and preprocessing.
   - Resizing frames and normalizing pixel values for model compatibility.
   
2. **Data Generator**:
   - Designed to handle large datasets efficiently.
   - Supports batch processing and dynamic augmentation for training.

3. **Model Architectures**:
   - **Conv3D**: Captures spatial and temporal features from video input.
   - **CNN + RNN**: Sequential processing of video frames using LSTMs combined with convolutional layers.
   - **Transfer Learning**: Leverages MobileNet for feature extraction from video frames.

4. **Evaluation and Visualization**:
   - Accuracy and loss metrics for each model.
   - Confusion matrix and classification reports for gesture predictions.
---

## Models

### Conv3D Models
- **Model 1**: 15 epochs, batch size 64, resolution (120x120), frames per video: 10
- **Model 2**: 20 epochs, batch size 20, resolution (50x50), frames per video: 6
- **Model 3**: 20 epochs, batch size 30, resolution (50x50), frames per video: 10
- **Model 4**: 25 epochs, batch size 50, resolution (120x120), frames per video: 10
- **Model 5**: 25 epochs, batch size 50, resolution (70x70), frames per video: 18

### CNN + RNN Model
- **Model 6**: 25 epochs, batch size 50, resolution (70x70), frames per video: 18

### Transfer Learning Using MobileNet
- **Model 7**: 15 epochs, batch size 5, resolution (120x120), frames per video: 18

---

## Results

- Each model's performance is evaluated on a validation set, and results are compared to determine the most efficient approach for real-time gesture recognition.

---

## Conclusion

The project demonstrates that deep learning techniques can effectively recognize gestures from video data, offering an intuitive way to interact with smart TVs.

---
