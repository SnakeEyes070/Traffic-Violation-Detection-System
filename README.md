# traffic-violation-detection

A computer vision system that detects traffic light violations using YOLO and CNN models. This system identifies vehicles running red lights and generates violation reports.

Features
Traffic Light Detection: YOLOv8 for real-time traffic light detection

Light State Classification: Custom CNN model classifies red/green/yellow lights

Violation Detection: Identifies vehicles passing during red lights

Web Interface: Upload videos and download processed results

Real-time Processing: Frame-by-frame analysis with visual annotations

traffic-violation-detection/
├── app.py                 # Main Flask web application
├── train.py              # Model training script
├── cnn.py               # CNN model architecture
├── requirements.txt     # Dependencies
├── models/             # Trained model weights
├── static/             # Uploads and outputs
└── templates/          # HTML templates

Local Installation
Clone the repository

bash
git clone https://github.com/yourusername/traffic-violation-detection.git
cd traffic-violation-detection
Install dependencies

bash
pip install -r requirements.txt
Train the model (optional)

bash
python train.py
Run the application

bash
python app.py
Open browser: http://localhost:5000

PythonAnywhere Deployment
Upload files to PythonAnywhere

Install requirements in virtual environment

Configure WSGI file with correct paths

Set up static files configuration

Reload web application

Usage
Upload Video: Select a traffic video (MP4/AVI)

Process: System detects traffic lights and vehicles

View Results: Download processed video with violations marked

Get Report: See total violations detected

Technologies
Computer Vision: OpenCV, YOLOv8

Deep Learning: PyTorch, CNN

Web Framework: Flask

Processing: NumPy, PIL

Model Details
Traffic Light Detection: YOLOv8n (COCO classes)

Classification Model: Custom CNN (7 classes)

Accuracy: 90%+ on validation set

Input Size: 32x32 or 64x64 RGB images

Limitations
Requires clear traffic light visibility

Works best with front-facing camera angles

Processing time depends on video length

CPU-only on PythonAnywhere (slower processing)

Future Improvements
License plate recognition

Multiple camera support

Real-time streaming

Mobile app interface

Cloud processing

Contributing
Fork the repository

Create a feature branch

Commit changes

Push to branch

Open Pull Request

License
MIT License - see LICENSE file for details

Support
For issues, please check:

Error logs in PythonAnywhere

File path configurations

Model file existence

Video format compatibility
