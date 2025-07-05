# Hand Tracking Module

This project provides a **Hand Tracking Module** designed for detecting and tracking hands in images or video streams. It leverages computer vision techniques to identify hand landmarks, enabling gesture recognition and interaction in real-time applications.

## Features

- Detects and tracks multiple hands simultaneously
- Identifies key hand landmarks (fingers, palm, etc.)
- Real-time performance suitable for live video processing
- Easy integration with other computer vision projects

## Usage

1. **Installation**  
    Clone the repository and install the required dependencies:
    ```bash
    git clone https://github.com/BertrandConxy/Hand-tracking-module.git
    cd Hand-tracking-module
    pip install -r requirements.txt
    ```

2. **Import and Use the Module**  
    ```python
    from HandTrackingModule import HandDetector

    cap = cv2.VideoCapture(0)
    detector = handDetector()
    while True:
        success, img = cap.read()
        img = detector.findHands(img)
        lmList = detector.findPosition(img)
        .... # Rest of the code
    ```

3. **Customization**  
    The module allows you to adjust detection confidence, maximum number of hands, and more.

## Applications

- Gesture-based user interfaces
- Sign language recognition
- Augmented reality
- Robotics and automation


## Acknowledgements

- Built using OpenCV and MediaPipe libraries.