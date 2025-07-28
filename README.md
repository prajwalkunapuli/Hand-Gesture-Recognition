# Hand Gesture Recognition

This project uses OpenCV and MediaPipe to recognize simple hand gestures from a webcam feed, such as "Thumbs Up" and "OK Sign".

## Features

- Real-time hand detection using MediaPipe
- Gesture recognition for "Thumbs Up" and "OK Sign"
- Displays gesture name on the video feed

## Requirements

- Python 3.x
- OpenCV (`opencv-python`)
- MediaPipe (`mediapipe`)

## Installation

1. Clone or download this repository.
2. Install dependencies:
   ```
   pip install opencv-python mediapipe
   ```

## Usage

1. Connect a webcam to your computer.
2. Run the script:
   ```
   python hand_gesture.py
   ```
3. A window will open showing the webcam feed and detected gestures.
4. Press `q` to exit.

## How It Works

- The script captures video from your webcam.
- MediaPipe detects hand landmarks.
- The code checks the position of the thumb and index finger to identify gestures:
  - **Thumbs Up:** Thumb tip is higher than index tip.
  - **OK Sign:** Thumb tip is close to index tip.