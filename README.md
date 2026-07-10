# 🚗 Autonomous Vehicle Dashboard

Real-time Autonomous Vehicle Dashboard with **YOLOv8**: object detection, tracking, lane segmentation, and trajectory prediction.

## 📖 Overview

This project is an **Autonomous Vehicle (AV) Dashboard** that demonstrates real-time 🎯 object detection, 🔄 tracking, 🛣️ lane segmentation, and 📈 trajectory prediction using **YOLOv8** and **ByteTrack**. It processes KITTI dataset images or your own driving videos and renders a visual dashboard with object velocity, predicted paths, and lane overlays.

## ✨ Features

- 🔍 **Object Detection** — detects cars, pedestrians, and cyclists using YOLOv8.
- 🎯 **Tracking** — tracks detected objects across frames using ByteTrack.
- 💨 **Velocity Estimation** — calculates approximate velocity (in pixels/frame) for each tracked object.
- 📈 **Trajectory Prediction** — predicts next positions of moving objects and plots their paths.
- 🛣️ **Lane Segmentation** — segments driving lanes using a YOLOv8 segmentation model.
- 🎥 **Video Output** — saves processed video with bounding boxes, trajectories, and lane overlays.

## 🛠️ Tech Stack

- 🐍 Python
- 🧠 Ultralytics YOLOv8 (detection + segmentation)
- 🔗 ByteTrack (multi-object tracking)
- 🎞️ OpenCV (`opencv-python-headless`)
- 🔥 PyTorch / TorchVision / TorchAudio
- 🔢 NumPy, Pillow, Matplotlib

## 📁 Project Structure

```
Autonomous-Vehicle-Dashboard-Project/
├── av_dashboard_project.py   # Main pipeline: detection, tracking, lane segmentation, dashboard overlay
├── requirements.txt          # Python dependencies
├── README.md                 # Project documentation
├── data/                     # Optional: place videos or KITTI dataset here
└── outputs/                  # Processed videos are saved here
```

## ✅ Requirements

- 🐍 Python 3.8+
- 📦 Libraries (see `requirements.txt`):
  - `ultralytics`
  - `opencv-python-headless`
  - `torch`
  - `torchvision`
  - `torchaudio`
  - `numpy`
  - `Pillow`
  - `matplotlib`
- 🗂️ KITTI dataset (optional — you can use your own driving video instead)

## 🚀 Usage

1. 📥 Clone the repository and install dependencies:

   ```bash
   git clone https://github.com/anushka-n2204/Autonomous-Vehicle-Dashboard-Project.git
   cd Autonomous-Vehicle-Dashboard-Project
   pip install -r requirements.txt
   ```

2. 🎬 Add your input video, or KITTI dataset images, to the `data/` folder.

3. ▶️ Run the pipeline:

   ```bash
   python av_dashboard_project.py
   ```

4. 📤 Find the processed video with detections, tracking IDs, trajectories, and lane overlays in `outputs/`.

> 💡 The pipeline also runs well in **Google Colab** — mount Google Drive, upload your video/dataset, install dependencies, and run the same steps end-to-end.

## 🖼️ Example Output

The processed video shows:

- 🟩 Bounding boxes around objects (cars, pedestrians, cyclists)
- 🔢 Object IDs and velocities
- 〰️ Trajectories (past positions)
- 🔮 Predicted next positions
- 🛣️ Lane segmentation overlay

## 📝 Notes

Built as a hands-on exploration of real-time perception for autonomous driving — combining object detection, multi-object tracking, semantic lane segmentation, and simple motion-based trajectory prediction into one live dashboard view.
