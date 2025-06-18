🚦 Traffic Red Light Violation Detection System
Using YOLOv8 | Python | OpenCV

This project detects vehicles running red lights using YOLOv8 for object detection and a rule-based system to identify violations.

📌 Features
Real-time detection of vehicles and traffic lights using YOLOv8.

Violation logging when a vehicle crosses the stop line during a red light.

Visual feedback with bounding boxes and violation alerts.

Exportable results (CSV/video).

⚙️ Installation
Clone the repository

bash
git clone https://github.com/mainakpal4/Traffic_Violation_YOLOv8.git
cd traffic-violation-detection
Install dependencies

bash
pip install ultralytics opencv-python pandas
(YOLOv8 requires ultralytics package)

Download YOLOv8 weights (or use custom-trained weights)

python
from ultralytics import YOLO
model = YOLO("yolov8n.pt")  # Nano model (smallest)


🚀 Usage
1. Run Detection on a Video
python
python detect.py --input input_video.mp4 --output output_video.avi
(Modify detect.py to adjust violation rules.)

3. Outputs
violations.csv: Timestamp, Vehicle ID, Confidence.

Annotated video with bounding boxes.

