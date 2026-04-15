# Hand Gesture Controller

This is a Python-based application that uses your computer's webcam and hand gestures to control various system functions such as mouse movement, clicking, scrolling, system volume, and screen brightness. It relies on OpenCV for video capture and MediaPipe for hand tracking and landmark mapping.

## Requirements
- Python 3.x
- An active Webcam

## Installation
Run the following command in your terminal to install the necessary libraries:
pip install opencv-python mediapipe PyAutoGUI comtypes pycaw protobuf screen-brightness-control

## How to Run
Navigate to the directory containing the file and execute the script using Python:
python testing.py

## Gestures and Controls
The application recognizes specific hand gestures to trigger mouse and system controls:

### Mouse Controls
- **V-Gesture (Index and Middle fingers extended and separated):** Moves the mouse cursor around the screen.
- **Fist:** Holds down the Left Mouse Button (useful for dragging/grabbing). Releasing the fist releases the drag.
- **Middle Finger Extended:** Performs a single Left Mouse Click.
- **Index Finger Extended:** Performs a single Right Mouse Click.
- **Two Fingers Closed (Index and Middle fingers extended and touching):** Performs a Double Click.

### Scrolling Controls
- **Pinch Minor (Pinching with your non-dominant/minor hand):** 
  - Move hand vertically (Up/Down) to scroll vertically.
  - Move hand horizontally (Left/Right) to scroll horizontally.

### Volume and Brightness Controls
- **Pinch Major (Pinching with your dominant/major hand):**
  - Move hand vertically (Up/Down) to adjust the System Volume.
  - Move hand horizontally (Left/Right) to adjust the Screen Brightness.

## Exiting the Application
To close the program smoothly, make sure the "Gesture Controller" camera window is actively selected (in-focus) and press the "Enter" key on your keyboard. You can also force close it by pressing `Ctrl + C` in the terminal from which you ran the script.
