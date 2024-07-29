# 3D Tracking of People from Multiple RGBD Cameras in an Operating Room

## Overview

This project focuses on developing a 3D tracking system to monitor individuals in an operating room using multiple RGBD cameras. The system combines deep learning and advanced computer vision techniques to ensure precise real-time tracking of medical professionals, which is crucial for workflow analysis, safety, and augmented reality support.

## Objectives

- Create a reliable system for tracking individuals in 3D using several RGBD cameras.
- Implement two methods for detection and tracking:
  - Deep Neural Networks (DNN) with a pre-trained Single Shot MultiBox Detector (SSD) model for face detection and dlib for facial landmark detection.
  - T and I pattern detection with a Histogram of Oriented Gradients (HOG) descriptor for pattern recognition.
- Ensure precise real-time tracking and calibration, creating a robust and adaptable system for operating room environments.

## Methodology

### Key Techniques
1. **Deep Neural Networks (DNN)**:
   - Used in conjunction with a pre-trained SSD model for real-time face detection.
   - Dlib library employed for accurate facial landmark detection.
2. **Integral Image Approach**:
   - Facilitates rapid computation of pixel value sums within sub-regions of images.
   - Identifies specific patterns such as "T" and "I" forms representing head and torso positions.
3. **Histogram of Oriented Gradients (HOG) Descriptor**:
   - Records the distribution of gradient orientations to ensure identified patterns match a human head.
4. **Socket-Based Communication System**:
   - Manages data transfer between multiple cameras and the central processing unit.
   - Ensures real-time processing and synchronization.
5. **Calibration**:
   - Achieved using techniques by Berthold K. P. Horn for accurate alignment of camera perspectives.
   - Matching algorithm ensures accurate correspondence of each monitored skeleton across multiple camera angles.

## Results

- The system demonstrated accurate real-time head tracking, effectively managing the dynamic environment of an operating room.
- Both DNN and HOG algorithms provided reliable identification and tracking of head positions.
- The project laid the groundwork for improved real-time tracking applications in healthcare, combining deep learning, advanced computer vision algorithms, and robust data communication protocols.

## Future Work

- Enhance the system's ability to monitor multiple individuals simultaneously.
- Improve management of coordinate adjustments when individuals cross paths.
- Develop more sophisticated pattern recognition methods to enhance accuracy at various distances.
- Integrate advanced filtering techniques like Kalman filters for improved stability and resilience.


