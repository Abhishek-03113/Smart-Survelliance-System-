# Smart Surveillance System

The **Smart Surveillance System** is a web application designed to provide real-time human detection and tracking capabilities using advanced computer vision techniques. Built with Python and the Flask web framework, this system leverages YOLO (You Only Look Once) models for object detection and tracking, making it suitable for various surveillance and monitoring applications.

---

## Features

- **Real-Time Human Detection**: Detects humans in video streams using a pre-trained YOLO model.
- **Object Tracking**: Tracks detected objects across frames with tracking algorithms like ByteTrack or BoTSORT.
- **Web-Based Interface**: Provides an intuitive web interface for interacting with the system.
- **Customizable Thresholds**: Allows users to set detection confidence thresholds.
- **Video Playback**: Supports video file input for detection and tracking.
- **Live Camera Feed**: Integrates with live camera feeds for real-time monitoring.
- **User Authentication**: Includes login and signup functionality for secure access.

---

## Prerequisites

Before running the application, ensure you have the following installed:

- Python 3.8 or higher
- pip (Python package manager)
- CUDA-enabled GPU (optional but recommended for faster inference)

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/Smart-Surveillance-System.git
   cd Smart-Surveillance-System
   ```

2. Install the required Python packages:

3. Download the pre-trained YOLO model:

4. Download the model from this link.

5. Place the downloaded model file (PersonsDetection.pt) inside the `Models/` directory.

---

## Usage

### Running the Application

- Open the project directory in your terminal.
- Start the Flask application.
- Open your web browser and navigate to `http://localhost:5000` (or the port specified in the terminal).

### Web Interface

- **Home Page**: Displays the main interface with options to start detection, tracking, and other features.
- **Video Stream**: Streams live video with real-time detection and tracking.
- **Login/Signup**: Securely log in or create an account to access the system.

---

## Project Structure

### Key Components

- `app.py`
  - Initializes the Flask application.
  - Configures the YOLO model for detection.
  - Defines routes for the web interface, including video streaming and user authentication.

- `HumanDetection.py`
  - Implements the `HumanDetection` and `Tracker` classes for object detection and tracking.
  - Uses the YOLO model for inference and OpenCV for video processing.

### Jupyter Notebooks

- `rtod.ipynb`: Real-time object detection experiments.
- `YOLOv8_TRAINING SCRIPT.ipynb`: Training scripts for YOLOv8.
- `yolo_v8.ipynb`: Additional experiments and testing.

---

## Configuration

- **Model Threshold**: Adjust the detection confidence threshold in `app.py` or `HumanDetection.py`.
- **Camera Index**: Change the camera index in `HumanDetection.py` or `app.py`.

---

## Troubleshooting

- **Camera Not Detected**: Ensure the correct camera index is used and the camera is connected.
- **Model Not Found**: Verify that the pre-trained model is placed in the `Models/` directory.
- **Slow Performance**: Use a CUDA-enabled GPU for faster inference.

---

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests to improve the project.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Acknowledgments

- Ultralytics YOLO for the YOLO model.
- Flask for the web framework.
- OpenCV for video processing.

