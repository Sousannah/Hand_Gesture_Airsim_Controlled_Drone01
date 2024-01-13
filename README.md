# Hand Gesture Control for AirSim Drone

## Overview
This repository demonstrates the control of a drone in the AirSim environment through hand gestures detected using the MediaPipe library. By employing computer vision techniques, the code interprets hand movements captured by the webcam to command the drone to perform specific actions.

## Features
- **Hand Gesture Recognition:** Utilizes MediaPipe's Hand module to detect and analyze hand landmarks in real-time from the webcam feed.
- **Drone Control:** Interprets recognized hand gestures to control the drone's movements in the AirSim simulator.
- **Gesture Mapping:** Maps specific finger configurations to predefined drone movements (e.g., up, down, left, right).
- **User Interface:** Displays a live feed with hand landmarks drawn and a label indicating the recognized gesture.

## Requirements
- Python 3.x
- OpenCV (cv2)
- MediaPipe (mediapipe)
- AirSim Python API (airsim)

## Installation
1. Clone this repository.
2. Install required libraries by running: `pip install -r requirements.txt`.

## Usage
1. Connect to AirSim: Ensure AirSim is running and connect to the simulator.
2. Run the Python script `airsim_hand_gesture_control.py`.
3. Perform hand gestures in front of your webcam.
4. The recognized gestures will control the drone's movements within the AirSim environment.

## Code Structure
This repository provides three distinct code files catering to different functionalities:

### 1. AirSim Integrated Control with Gesture Recognition
- **File Name:** `airsim_hand_gesture_control.py`
- **Description:** Integrates hand gesture recognition using MediaPipe and control commands for the drone in the AirSim environment. Detects hand gestures from the webcam feed using MediaPipe's Hand module and maps these gestures to specific movements for the drone.

### 2. MediaPipe Hand Gesture Recognition Only
- **File Name:** `mediapipe_hand_gesture.py`
- **Description:** Focuses solely on hand gesture recognition using MediaPipe's Hand module. Captures the webcam feed, detects hand landmarks in real-time, and displays the hand landmarks with associated labels indicating the recognized gestures. This code does not involve AirSim integration and serves as a standalone demonstration of hand gesture recognition.

### 3. AirSim Controlled Drone with Limitations
- **File Name:** `airsim_limitations.py`
- **Description:** Provides a simplified version of the AirSim integration for controlling the drone based on hand gestures. While still utilizing hand gesture recognition from MediaPipe, this script imposes certain limitations on the drone's movements to ensure safer operation.

Users can choose the script based on their requirements:
- Use `airsim_hand_gesture_control.py` for integrating hand gesture control with the AirSim simulator.
- Use `mediapipe_hand_gesture.py` for a standalone demonstration of hand gesture recognition without drone control functionalities.
- Use `airsim_limitations.py` for a version with added limitations on drone movements for safety.

This section clarifies the purpose and functionality of each code file, allowing users to select the appropriate script based on their specific needs—whether it's controlling a drone in AirSim, exploring hand gesture recognition, or implementing safety measures in drone control.

## Acknowledgments
- **AirSim:** Utilized for the drone simulation environment.
- **MediaPipe:** Used for real-time hand landmark detection.
- **OpenCV:** Employed for image processing and webcam capture.

## License
This project is licensed under the MIT License.

## Contribution
Contributions are welcome! Feel free to fork this repository, create pull requests, or open issues for any improvements, bug fixes, or suggestions.
