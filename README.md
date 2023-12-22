# Real-Time Face Mask Detection

## Overview
This Python script utilizes a pre-trained face detection model and a face mask detection model to perform real-time face mask detection using a live video stream. The face mask detection model determines whether a person in the video is wearing a mask or not.

## Prerequisites
- Python
- OpenCV
- TensorFlow
- imutils

## How to Use
1. Install the required dependencies:
    ```bash
    pip install opencv-python tensorflow imutils
    ```
2. Download the face detection model files:
   - [deploy.prototxt](face_detector/deploy.prototxt)
   - [res10_300x300_ssd_iter_140000.caffemodel](face_detector/res10_300x300_ssd_iter_140000.caffemodel)
3. Download the face mask detection model file:
   - [mask_detector.model](mask_detector.model)
4. Run the Python script:
    ```bash
    python face_mask_detection.py
    ```
5. Press `q` to exit the application.

## Model Details
- **Face Detection Model**: Utilizes a pre-trained face detection model from OpenCV (`deploy.prototxt` and `res10_300x300_ssd_iter_140000.caffemodel`).
- **Face Mask Detection Model**: Uses a deep learning model trained to detect face masks.

## Video Stream
The script uses the OpenCV VideoStream class to capture frames from the default camera (`src=0`). Adjust the source (`src`) if you have multiple cameras.

## Controls
- Press `q` to exit the application.

Feel free to customize this README according to your specific needs and provide any additional details that may be helpful for users. Include information about the models used, the purpose of the application, and any special considerations.

## dataset https://www.kaggle.com/datasets/andrewmvd/face-mask-detection
