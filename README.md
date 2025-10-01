# Smart Child Safety Monitoring System in Vehicles

---

## **Project Overview**
This system uses **object detection** and **age estimation** models to monitor vehicle cabins in real-time. It is designed to prevent accidents related to children being left in cars. Key features include:

- Detects **children, adults, and pets** in vehicles.
- Estimates **age groups** of occupants using deep learning.
- Sends **alerts** (e.g., notifications) if a child is detected alone in the car.
- Uses **YOLOv8/YOLOv9/YOLOv10** for object detection and **EfficientNet** for age estimation.
- Implemented in **Python** using **Google Colab** for training and testing models.

---

## **Datasets**
The system uses in-cabin vehicle datasets containing images of:

- Children (`kid`)
- Adults (`adult`)
- Pets (`pet`)

The dataset is split into:

- **70% training**  
- **15% validation**  
- **15% testing**

---

## **Deep Learning Models Used**
1. **Object Detection:** YOLOv8m, YOLOv9m, YOLOv10m  
2. **Age Estimation:** EfficientNet-B4  
3. **Face Detection:** MTCNN  
4. **Alert System:** WhatsApp notifications (optional integration)  

---

## **Installation & Setup**
1. Open the project in **Google Colab**.
2. Ensure required libraries are installed:
   ```bash
   pip install torch torchvision mtcnn efficientnet_pytorch yolov8
