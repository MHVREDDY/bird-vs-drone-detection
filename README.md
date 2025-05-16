# Bird vs Drone Detection Using YOLOv5

## 📌 Project Overview

This project focuses on distinguishing between birds and drones using deep learning techniques, specifically the YOLOv5 object detection model. It was developed to address the growing challenges of drone surveillance and safety, especially in sensitive areas like airports, military zones, and wildlife habitats.

## 🧠 Objective

To build an accurate, efficient, and real-time object detection system that classifies flying objects as either **birds** or **drones** using a custom-trained YOLOv5 model.

## 🛠️ Technologies Used

- **YOLOv5**: You Only Look Once v5 for object detection.
- **Python**: Primary programming language.
- **OpenCV**: For video and image processing.
- **PyTorch**: Deep learning framework.
- **LabelImg**: For manual image annotation.
- **Google Colab / Local Jupyter Notebook**: Training and testing environment.

## 📂 Dataset

- **Custom Dataset**: Containing labeled images of birds and drones.
- **Image Format**: `.jpg` images with corresponding `.txt` YOLO format labels.
- **Annotation Tool**: LabelImg.

## ⚙️ Model Training

- Model: YOLOv5s (small version for faster training)
- Training Epochs: 100 (adjustable)
- Batch Size: 16
- Optimizer: SGD/Adam
- Loss Function: YOLOv5 built-in object detection loss
- Dataset Split: 80% training, 20% validation

## 📈 Evaluation Metrics

- **mAP@0.5**: Mean Average Precision at IoU 0.5
- **Precision & Recall**
- **F1 Score**

## 🚀 Features

- Real-time detection from webcam.
- High precision for both classes.
- Lightweight and fast inference.

## 🖼️ Sample Outputs

> *Include screenshots or gifs here showing detection bounding boxes around birds and drones.*

## 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bird-vs-drone-yolov5.git
   cd bird-vs-drone-yolov5
2. Install dependencies:
   pip install -r requirements.txt
3. Run detection on an image:
   python detect.py --weights runs/train/exp/weights/best.pt --source your_image.jpg
4.Future Scope:
   Expand dataset with more diverse images
   Deploy on edge devices (Raspberry Pi, Jetson Nano).
   Extend to multi-class detection (e.g., other flying objects).
