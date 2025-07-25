# 🚦 Smart Pedestrian and Vehicle Detection System

This project uses a **pre-trained MobileNet-SSD model** to detect persons and vehicles in a video and simulate a **smart traffic signal system** based on real-time majority detection.


## 📌 Overview

The system:
- 🎥 Takes a **video input**
- 🧠 Detects objects **frame-by-frame** using MobileNet-SSD
- 🔢 Counts the number of **persons** and **vehicles** in each frame
- 🚦 Displays a 🟢 green, 🔴 red, or 🟡 yellow **signal indicator** based on the group in majority
- 💾 Outputs a **video with bounding boxes, labels, and signal indicators**


## 🧠 Features

- 🎯 Real-time **object detection** using OpenCV's DNN module  
- ⚡ Fast inference with **MobileNet-SSD (Caffe model)**  
- 🔁 Simple yet effective **decision-making logic** to simulate smart signal control  
- 🖼️ **Visual overlays**: bounding boxes, confidence scores, labels, and signal circles  


## 🛠️ Technologies Used

- Python  
- OpenCV  
- MobileNet-SSD (Caffe Model)  
- Google Colab (for execution & demo)  


## 📽️ How It Works

1. 📤 Upload a `.mp4` **video file** via Google Colab  
2. 🧠 The script processes **every alternate frame**:
   - Detects objects like `person`, `car`, `bus`, `motorbike`, etc.
   - Counts **detected persons and vehicles**
   - Adds **bounding boxes**, **labels**, and **confidence scores**
   - Displays a **traffic signal** indicator: 🟢 / 🔴 / 🟡
3. 🎞️ Saves and allows download of the **output video**


## 📁 Project Files

- `MobileNetSSD_deploy.prototxt` – Model configuration  
- `MobileNetSSD_deploy.caffemodel` – Pre-trained weights  
- `output_video_with_signal.mp4` – Final processed output video  


## 🖼️ Output Behavior

- 🟢 **More persons** → _"All clear!"_  
- 🔴 **More vehicles** → _"Stay safe!"_  
- 🟡 **Equal count** → _"Proceed with caution!"_



## 🚀 Run on Google Colab

1. Upload your `.mp4` video  
2. Run all notebook cells:
   - 📥 **Download and load** the model  
   - 🧠 **Perform detection**
   - 🎞️ **Save and download** the output video  
3. 🎬 View or share your **smart detection video**



## 📈 Possible Future Enhancements

- 🔄 Upgrade to **YOLOv8 or TensorFlow Lite** for faster and more accurate detection  
- 🧾 **Log detection data** to a `.csv` for analysis  
- 📊 Build a simple **dashboard** to visualize detection statistics  
- 📷 Add support for **real-time webcam-based detection**
