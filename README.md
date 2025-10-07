# DRONE-recognition-trained-
A drone recognition model trained to identify and classify different types of drones in real-time, enhancing surveillance, security, and aerial monitoring applications
🛸 YOLOv11 Drone Detection

A real-time drone detection system using YOLOv11 and your custom-trained model.

 Features

Live detection via webcam

Trained with custom drone dataset

Real-time bounding boxes and confidence display

Simple and lightweight Python script

 Requirements

Python 3.8 or higher

VS Code (recommended)

Dependencies:pip install ultralytics opencv-python matplotlib
 Setup
Clone or download this project.

Place your trained model file (best.pt) in the project folder.

Create a Python file named detect.py and add:

python
Copy code
from ultralytics import YOLO

model = YOLO("best.pt")
results = model.predict(source=0, show=True, conf=0.5)
Run in terminal:

bash
Copy code
python detect.py
 Output
Live webcam feed with detected drones highlighted.

Saved results are stored in runs/detect/predict/.

Tips
Increase accuracy by adding more drone and background images.

"""Adjust detection threshold using conf=0.5 (try 0.6 or 0.7 for stricter detection).
The YOLOv11 model used in this project was trained for 50 epochs on a custom dataset containing over 40,000 images of drones captured from various angles, lighting conditions, and backgrounds. The dataset also included negative samples (non-drone images) to help the model distinguish drones from other objects and reduce false detections. This extensive training enabled the model to achieve high accuracy and strong generalization performance for real-time drone detection tasks."""

 License
This project is open for educational and personal use.the trained model is in the github named best.pt or use link->https://github.com/daya-cpu/DRONE-recognition-trained-/blob/main/best.pt Please use this model responsibly







