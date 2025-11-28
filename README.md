🚦 Smart Traffic Management Using YOLOv3

This project implements an AI-powered traffic monitoring system using YOLOv3, enabling automated detection of vehicles from live traffic images. The goal is to support smart city applications such as:
	•	Traffic density analysis
	•	Automated signal timing
	•	Real-time monitoring
	•	Congestion alerts

⸻

📌 Features

✔ YOLOv3 Object Detection

Detects vehicles such as:
	•	Cars
	•	Trucks
	•	Buses
	•	Motorcycles
	•	Bicycles

✔ Multi-direction Traffic Images

Includes sample images of traffic from:
	•	East
	•	West
	•	North
	•	South

✔ Easy to Run

Simply load the YOLOv3 model → run the script → get detections.

⸻

🗂 Project Structure

SMART-TRAFFIC-MANAGEMENT/
│── code_1.py              # Main Python script (YOLOv3 detection)
│── coco.names             # Object class names
│── yolov3.cfg             # YOLOv3 model configuration
│── yolov3.weights         # (Ignored in GitHub) Pre-trained model weights
│── east_traffic.jpeg
│── west_traffic.jpeg
│── north_traffic.jpeg
│── south_traffic.jpeg
│── README.md              # Documentation
└── .gitignore             # Ignores large model weights

⚠️ yolov3.weights is large (~200MB), so it is not uploaded to GitHub
A download link is provided below.

📥 Download YOLOv3 Weight File

You must download the YOLOv3 pre-trained model manually:

YOLOv3 Weights (Official):
https://pjreddie.com/media/files/yolov3.weights

After downloading, place the yolov3.weights file in the project folder.

⸻

🛠 Installation & Setup

1️⃣ Install dependencies

Open terminal in the project folder:
pip install opencv-python numpy

2️⃣ Ensure YOLOv3 files exist

Required files in project directory:
yolov3.cfg
yolov3.weights
coco.names

3️⃣ Run the program

python code_1.py

📸 Output

The script displays:
	•	Detected vehicles
	•	Bounding boxes
	•	Traffic density estimation
	•	Processed images with annotations

⸻

🔍 How It Works
	1.	Load YOLOv3 model via OpenCV’s DNN module
	2.	Read input traffic images
	3.	Preprocess → blob → forward pass through YOLO
	4.	Extract detected vehicles
	5.	Draw bounding boxes
	6.	Count vehicles per frame
	7.	Output results

⸻

🚧 Future Improvements
	•	Integrate live CCTV video feed
	•	Deploy as a Flask web app
	•	Use YOLOv5/YOLOv8 for better accuracy
	•	Add traffic signal timing optimization

⸻

👨‍💻 Author

Jeevan
Smart AI-based Traffic Management System
YOLOv3 + OpenCV
