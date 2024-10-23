# Self-Driving-Car-using-IoT-Machine-Learning-and-CNN
This project demonstrates the implementation of a self-driving car prototype using IoT technology, Machine Learning, and Convolutional Neural Networks (CNNs). The model processes data from sensors and a camera to enable autonomous navigation and obstacle avoidance.
## Project Overview
The self-driving car prototype collects data from various sensors (such as ultrasonic sensors, cameras, etc.) to autonomously navigate its environment. A CNN-based machine learning model is used to process visual data and detect obstacles, traffic signs, and lane markings, while IoT ensures real-time data transmission for remote monitoring.

## Features
    Autonomous Navigation: The car navigates based on sensor and camera inputs.
    Obstacle Detection: Uses sensor data to avoid collisions.
    Lane Detection: CNN-based model helps detect lanes.
    Remote Monitoring: IoT integration allows monitoring and control via a cloud platform or smartphone.

## Software Required
    Python (for developing the machine learning model and IoT functionality)
    OpenCV (for image processing tasks)
    Keras/TensorFlow (for CNN implementation)
    Flask/Django (for the IoT dashboard or monitoring system)
    Raspberry Pi OS (or other suitable OS for Raspberry Pi)
    Arduino IDE (if using additional microcontrollers)
## System Architecture
  The system consists of:

    Sensors: Ultrasonic sensors for obstacle detection.
    Camera: To capture live video feed for lane detection and object recognition.
    CNN Model: A pre-trained CNN model processes images and predicts actions (e.g., stop, turn left/right).
    Motor Control: The system sends commands to the motor driver module based on predictions.
    IoT: Monitors real-time data and allows control through a web interface.
## Data Flow Diagram

  ![image](https://github.com/user-attachments/assets/5dc3fb8d-6fa6-472f-8d07-eb4de60e105d)


## Installation and Setup
  Clone this Repository:

    git clone https://github.com/your-username/Self-Driving-Car-IoT-ML-CNN.git
## Set up Raspberry Pi:

  Install Raspberry Pi OS and ensure the camera module and sensors are connected properly.
  Install Python dependencies:
    sudo apt-get update
    sudo apt-get install python3-pip
    pip3 install tensorflow keras opencv-python flask
    
## Configure IoT Platform:

  Set up an IoT platform (such as ThingSpeak or Firebase) to monitor and control the car remotely.
## How It Works
    Step 1: The camera captures a video feed and ultrasonic sensors measure distances.
    Step 2: The CNN model processes the video feed to identify lanes, obstacles, and traffic signs.
  ![Screenshot_2024-10-23-22-38-46-27_965bbf4d18d205f782c6b8409c5773a4](https://github.com/user-attachments/assets/ec7c5f65-8725-4305-a4f1-fdacb895ef54)

    Step 3: Based on the processed data, the car makes decisions such as moving forward, turning, or stopping.
    Step 4: IoT integration allows remote monitoring and control through a web interface.


## Model Training
  Dataset
  A custom dataset of road images with labeled lanes, obstacles, and traffic signs was used to train the CNN model.
  You can expand the model by training on more images using platforms like Kaggle or custom-collected datasets.
  Training Process
  The model was trained using a Convolutional Neural Network (CNN) for image classification and lane detection.
  TensorFlow/Keras was used for the model, which was trained on a dataset of labeled road images.

## Hardware Used
    Raspberry Pi (or any suitable microcontroller for IoT applications)
    Ultrasonic Sensors (for obstacle detection)
    Camera Module (for visual input)
    Motor Driver Module
    DC Motors and chassis
    Wi-Fi Module (for IoT connectivity)
    Power Supply/Battery
    Jumper Wires and Breadboard (for prototyping)
