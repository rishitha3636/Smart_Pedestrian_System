🚦 Smart Pedestrian and Vehicle Detection System
This project uses a pre-trained MobileNet-SSD model to detect persons and vehicles in a video and simulate a smart signaling system (like traffic lights) based on majority detection.

📌 Overview
The system:

Takes a video input.
Detects objects frame-by-frame using MobileNet-SSD.
Counts the number of persons and vehicles in each frame.
Displays a 🟢 green, 🔴 red, or 🟡 yellow circle to simulate a traffic signal based on which group is in majority.
Generates an output video with bounding boxes, labels, and signal indicators.
🧠 Features
🎯 Real-time object detection using OpenCV's DNN module.
⚡ Fast inference using MobileNet-SSD (Caffe model).
🔁 Simple decision-making logic to simulate smart signal control.
🖼️ Visual overlays: bounding boxes, labels, and traffic-like signal circles.
🛠️ Technologies Used
Python
OpenCV
MobileNet-SSD (Caffe Model)
Google Colab (for demonstration & execution)
📽️ How It Works
Upload a video file via Google Colab.

The script processes every alternate frame:

Detects objects like person, car, bus, motorbike, etc.
Counts detected persons and vehicles.
Adds bounding boxes and confidence scores.
Displays signal indicator (🟢 / 🔴 / 🟡) based on counts.
Saves and allows download of the output video.

📁 Project Files
MobileNetSSD_deploy.prototxt – Model configuration file
MobileNetSSD_deploy.caffemodel – Pre-trained weights
output_video_with_signal.mp4 – Final processed video with detection and signal overlay
🖼️ Output Behavior
🟢 More persons → "All clear!" 🔴 More vehicles → "Stay safe!" 🟡 Equal → "Proceed with caution!"

🚀 Run on Google Colab
Upload your video in .mp4 format.

Run all the notebook cells:

📥 Download and load model
🧠 Perform detection
🎞️ Save and download output video
View or share your smart detection video.

📈 Possible Future Enhancements
🔄 Switch to YOLOv8 or TensorFlow Lite for faster and more accurate detection.
🧾 Log detection data to a .csv file for analysis.
📊 Build a simple dashboard to visualize detection stats.
📷 Add support for real-time webcam-based detection.
