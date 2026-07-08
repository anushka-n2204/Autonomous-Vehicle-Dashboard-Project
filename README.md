# Autonomous Vehicle Dashboard
Real-time Autonomous Vehicle Dashboard with YOLOv8: Object detection, tracking, lane segmentation, and trajectory prediction.

# Autonomous Vehicle Dashboard Project

## Overview
This project is an **Autonomous Vehicle (AV) Dashboard** that demonstrates real-time **object detection, tracking, lane segmentation, and trajectory prediction** using **YOLOv8** and **ByteTrack**. It processes KITTI dataset images or your own driving videos and provides a visual dashboard with object velocity, predicted paths, and lane overlays.

---

## Features

- **Object Detection:** Detects cars, pedestrians, and cyclists using YOLOv8.
- **Tracking:** Tracks detected objects across frames using ByteTrack.
- **Velocity Estimation:** Calculates approximate velocity (in pixels/frame) for each tracked object.
- **Trajectory Prediction:** Predicts next positions of moving objects and shows their paths.
- **Lane Segmentation:** Segments driving lanes using YOLOv8 segmentation model.
- **Video Output:** Saves processed video with bounding boxes, trajectories, and lane overlays.

---

## Project Structure
AV_Dashboard_Project/
├── AV_Dashboard.ipynb # Main Colab notebook
├── README.md # Project documentation
├── requirements.txt # Python dependencies
├── data/ # Optional: Place videos or KITTI dataset here
└── outputs/ # Processed videos will be saved here


---

## Requirements

- Python 3.8+
- Libraries:
  ultralytics
  opencv-python-headless
  torch
  torchvision
  torchaudio

  - KITTI dataset (optional, can use your own video)

---

## Usage

1. **Open the notebook** `AV_Dashboard.ipynb` in Google Colab.  
2. **Mount Google Drive** to store videos and outputs.  
3. **Upload videos** in your Drive folder or use KITTI dataset images.  
4. **Run cells sequentially**:  

 - Install dependencies  
 - Download and verify dataset  
 - Load YOLOv8 models  
 - Run object detection and lane segmentation  
 - Process videos with tracking and dashboard overlay  

5. **Download the output video** from `/content/AV_Dashboard_Output.mp4`.

---

## Example Output

- Processed video will show:  
- Bounding boxes around objects (cars, pedestrians, cyclists)  
- Object IDs and velocities  
- Trajectories (past positions)  
- Predicted next positions  
- Lane segmentation overlay  





