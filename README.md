# 🌱 **YOLOv8 Custom Dataset Training**

Train a YOLOv8 object detection model on a custom dataset using Google Colab, Roboflow, and the Ultralytics YOLOv8 framework.

This project demonstrates an end-to-end workflow for preparing data, training a detection model, validating results, and running predictions — all inside a single Colab notebook.

---

## 📘 **Overview**

This project shows how to:

- Import a custom dataset from **Roboflow**
- Install and configure **YOLOv8**  
- Train a YOLOv8 model on your custom images  
- Validate model performance  
- Run predictions and visualize outputs  

The notebook is fully automated and easy to adapt to any custom object detection task.

---

## 🛠️ **Tech Stack**

- **Google Colab** – training environment  
- **Python**  
- **Ultralytics YOLOv8**  
- **Roboflow** (dataset hosting + YOLOv8 export)  
- **CUDA GPU** for accelerated training  

---

## 🚀 **Training Pipeline**

1. **Setup Environment**  
   - Install Ultralytics YOLOv8  
   - Install Roboflow SDK  

2. **Load the Dataset**  
   - Authenticate with Roboflow  
   - Download dataset in YOLOv8 format  

3. **Train the Model**  
   ```bash
   yolo task=detect mode=train model=yolov8m.pt data=path/to/data.yaml epochs=30 imgsz=640
