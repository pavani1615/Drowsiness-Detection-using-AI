# Drowsiness-Detection-using-AI
Drowsiness is one of the major causes of road and workplace accidents. This project implements a real-time AI-based drowsiness detection system that monitors eye activity through a webcam and generates instant voice alerts when prolonged eye closure is detected.
A real-time drowsiness detection system that uses computer vision and facial landmarks to detect when a driver is getting drowsy. The system monitors eye movements and triggers an alert when signs of drowsiness are detected.

## Features

- Real-time face detection and tracking
- Eye aspect ratio (EAR) calculation for drowsiness detection
- Visual feedback with facial landmark visualization
- Audio alerts when drowsiness is detected
- Simple and intuitive interface

## Requirements

- Python 3.7+
- OpenCV
- MediaPipe
- SciPy
- pyttsx3

## Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/Drowsiness-Detection-Using-AI.git
cd Drowsiness-Detection-Using-AI
```

2. Install the required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Run the application:
```bash
python app.py
```

2. The program will access your webcam and start monitoring your face.
3. The system will display a window showing your face with facial landmarks.
4. When drowsiness is detected (eyes closed for a certain duration), an audio alert will be triggered.
5. Press 'q' to quit the application.

## How it Works

The system uses the following approach to detect drowsiness:

1. Face Detection: Uses MediaPipe Face Mesh to detect facial landmarks
2. Eye Tracking: Monitors specific landmarks around the eyes
3. EAR Calculation: Computes the Eye Aspect Ratio (EAR) to determine if eyes are closed
4. Alert System: Triggers audio alerts when sustained eye closure is detected

## Parameters

- `EAR_THRESHOLD`: Threshold for eye aspect ratio (default: 2)
- `EAR_CONSEC_FRAMES`: Number of consecutive frames below threshold to trigger alert (default: 48)

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is licensed under the MIT License - see the LICENSE file for details.
