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

1. **Data Generation**: Custom generator logic for handling video frames and feeding them into the models.
2. **Models**:
   - **Conv3D**: Designed to handle spatial and temporal aspects of video data.
   - **CNN + RNN**: Combines convolutional layers with LSTM for sequential frame analysis.
   - **MobileNet (Transfer Learning)**: Utilizes pre-trained MobileNet for feature extraction.
3. **Evaluation**: Performance comparison of different models on metrics like accuracy and loss.

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

## Usage Instructions

1. **Clone the Repository**:
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```
