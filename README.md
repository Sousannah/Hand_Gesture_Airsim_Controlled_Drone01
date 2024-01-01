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

### Code Structure
- **`airsim_hand_gesture_control.py`:** Main script integrating hand gesture recognition and drone control.
- **`requirements.txt`:** Lists necessary Python libraries and versions.

### Acknowledgments
- **AirSim:** Utilized for the drone simulation environment.
- **MediaPipe:** Used for real-time hand landmark detection.
- **OpenCV:** Employed for image processing and webcam capture.

### License
This project is licensed under [MIT License](LICENSE).

### Contribution
Contributions are welcome! Feel free to fork this repository, create pull requests, or open issues for any improvements, bug fixes, or suggestions.

---

This overview provides a concise yet informative summary of the project, covering its purpose, features, requirements, usage instructions, code structure, acknowledgments, licensing, and encouragement for contributions.
