# Hand_Gesture_Airsim_Controlled_Drone01

### Overview
This repository provides a demonstration of controlling a drone in the AirSim environment using hand gestures detected via the MediaPipe library. By utilizing computer vision techniques, the code interprets hand movements captured by the webcam to command the drone to perform specific actions.

### Features
- **Hand Gesture Recognition:** Utilizes MediaPipe's Hand module to detect and analyze hand landmarks in real-time from the webcam feed.
- **Drone Control:** Interprets recognized hand gestures to control the drone's movements in the AirSim simulator.
- **Gesture Mapping:** Maps specific finger configurations to predefined drone movements (e.g., up, down, left, right).
- **User Interface:** Displays a live feed with hand landmarks drawn and a label indicating the recognized gesture.

### Requirements
- Python 3.x
- OpenCV (`cv2`)
- MediaPipe (`mediapipe`)
- AirSim Python API (`airsim`)

### Installation
1. Clone this repository.
2. Install required libraries by running: `pip install -r requirements.txt`.

### Usage
1. Connect to AirSim: Ensure AirSim is running and connect to the simulator.
2. Run the Python script `airsim_hand_gesture_control.py`.
3. Perform hand gestures in front of your webcam.
4. The recognized gestures will control the drone's movements within the AirSim environment.

Certainly! Here's an additional section for your repository README to explain the structure involving two different code files, one dedicated to AirSim control and the other focused solely on MediaPipe for hand gesture recognition.

---

## Code Structure

This repository provides three distinct code files catering to different functionalities:

### AirSim Integrated Control with Gesture Recognition
**File Name:** `airsim_hand_gesture_control.py`  
**Description:** This script integrates both hand gesture recognition using MediaPipe and control commands for the drone in the AirSim environment. It detects hand gestures from the webcam feed using MediaPipe's Hand module and maps these gestures to specific movements for the drone (e.g., up, down, left, right) within the AirSim simulator.

### MediaPipe Hand Gesture Recognition Only
**File Name:** `mediapipe_hand_gesture.py`  
**Description:** This script focuses solely on hand gesture recognition using MediaPipe's Hand module. It captures the webcam feed, detects hand landmarks in real-time, and displays the hand landmarks with associated labels indicating the recognized gestures. This code does not involve AirSim integration and serves as a standalone demonstration of hand gesture recognition.

### AirSim Controlled Drone with Limitations
**File Name:** `airsim_limitations.py`  
**Description:** This script provides a simplified version of the AirSim integration for controlling the drone based on hand gestures. While still utilizing hand gesture recognition from MediaPipe, this script imposes certain limitations on the drone's movements to ensure safer operation. For instance, it limits the duration or distance of certain actions, preventing continuous or excessive maneuvers. Users can refer to this script as a starting point for implementing safety measures in their own projects.

Users can choose the script based on their requirements:

- Use `airsim_hand_gesture_control.py` for integrating hand gesture control with the AirSim simulator.
- Use `mediapipe_hand_gesture.py` for a standalone demonstration of hand gesture recognition without drone control functionalities.
- Use `AirSim_Controlled_Drone_With_Limitations.py` for a version with added limitations on drone movements for safety.

This section clarifies the purpose and functionality of each code file, allowing users to select the appropriate script based on their specific needs—whether it's controlling a drone in AirSim, exploring hand gesture recognition, or implementing safety measures in drone control.

### Acknowledgments
- **AirSim:** Utilized for the drone simulation environment.
- **MediaPipe:** Used for real-time hand landmark detection.
- **OpenCV:** Employed for image processing and webcam capture.

### License
This project is licensed under [MIT License](LICENSE).

### Contribution
Contributions are welcome! Feel free to fork this repository, create pull requests, or open issues for any improvements, bug fixes, or suggestions.

