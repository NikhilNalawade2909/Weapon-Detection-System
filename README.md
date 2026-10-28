# Weapon Detection System Using YOLOv3 and OpenCV

A computer vision-based Weapon Detection System developed using **Python, OpenCV, and YOLOv3**. The project is designed to detect potential weapons in images or video streams using deep learning-based object detection.

## Project Overview

The primary objective of this project is to demonstrate how computer vision and object detection techniques can be applied to identify weapons in visual data.

The system processes input frames using OpenCV and a YOLOv3 model to identify objects and display detection results with bounding boxes.

## Technologies Used

- **Programming Language:** Python
- **Computer Vision:** OpenCV
- **Deep Learning Model:** YOLOv3
- **Web Technologies:** HTML, CSS, JavaScript
- **Web Framework:** Flask
- **Version Control:** Git and GitHub

## Key Features

- Weapon detection using YOLOv3
- Image and video frame processing
- Webcam input support
- Bounding box visualization
- Configurable YOLO model and class labels
- Python-based detection scripts

## Project Structure

```text
Weapon-Detection-System/
├── assets/
├── static/
├── templates/
├── infer2.py
├── infere.py
├── main.py
├── yolo.names
├── yolov3_testing.cfg
├── yolov3_testing2.cfg
├── README.md
└── .gitignore
```

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/NikhilNalawade2909/Weapon-Detection-System.git
cd Weapon-Detection-System
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```cmd
venv\Scripts\activate
```

### 3. Install Required Libraries

```bash
pip install opencv-python numpy
```

Additional dependencies may be required depending on the script being executed.

### 4. Add YOLOv3 Model Weights

Place the trained model weights file in the project root directory:

```text
yolov3_training_2000.weights
```

**Note:** The weights file is excluded from GitHub because it exceeds GitHub's standard file size limit. The project requires a compatible trained weights file to perform detection.

### 5. Run Weapon Detection

For webcam detection, execute:

```bash
python infer2.py -i 0 -c yolov3_testing.cfg -w yolov3_training_2000.weights -cl yolo.names
```

Use `0` for the default webcam. Ensure the configuration, weights, and class labels correspond to the same trained model.

## How It Works

1. The application receives input from a camera or supported media source.
2. OpenCV processes the input frames.
3. The YOLOv3 model analyzes the frames to detect objects.
4. The system identifies detections according to the model's trained classes.
5. Bounding boxes are displayed around detected objects.

## Learning Outcomes

This project provided practical exposure to:

- Python programming
- Computer vision and image processing
- Deep learning-based object detection
- YOLO model configuration
- Working with trained model weights
- Debugging and testing detection scripts

## Future Enhancements

- Email alerts when potential weapons are detected
- Improved detection accuracy with additional training data
- Real-time monitoring dashboard
- Detection event logging
- Deployment as a web application

## Author

**Nikhil Nalawade**

B.E. Information Technology  
Sinhgad Institute of Technology, Lonavala

GitHub: https://github.com/NikhilNalawade2909

## Disclaimer

This project is intended for educational and research purposes. Automated weapon detection can produce false positives and false negatives and should not be relied upon as a standalone security system.
