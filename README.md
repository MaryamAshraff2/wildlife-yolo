# Wildlife Detection and Classification using YOLOv8  

## Overview  
This project focuses on developing a real-time wildlife detection and classification system using **YOLOv8**. The system is trained on a **custom dataset** to detect and classify various wild animals from images and live video feeds. The model is optimized for real-time object detection, making it suitable for conservation efforts, wildlife monitoring, and research applications.  

## Features  
- **Real-Time Detection**: Uses YOLOv8 for fast and accurate object detection.  
- **Custom Training**: Includes additional species beyond the pretrained model.  
- **Bounding Box and Labels**: Displays detected animals with labeled bounding boxes.  
- **Live Camera Integration**: Supports real-time detection via webcam or external video feeds.  
- **Optimized Performance**: Trained on Google Colab with a balanced dataset to enhance accuracy.  

## Dataset  
- **Pretrained Model**: Initially tested with `yolov8s.pt` on four species (*Bear, Zebra, Giraffe, Elephant*).  
- **Custom Training**: Added **Lion** and **Tiger** using a dataset from Roboflow.  
- **Dataset Structure**:  
  - **Training**: 690 images  
  - **Validation**: 100 images  
  - **Testing**: 190 images  

## Training Setup  
- **Platform**: Google Colab  
- **Model**: YOLOv8  
- **Training Parameters**:  
  - `epochs=50`  
  - `imgsz=640`  
  - `batch=8`  
  - `device="cpu"` (due to GPU limits)  

## Installation  
### Prerequisites  
Ensure Python is installed along with the required dependencies.  

```bash
pip install ultralytics opencv-python numpy

