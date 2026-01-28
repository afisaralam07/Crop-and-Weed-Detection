#  Crop & Weed Detection using YOLOv8

##  Project Overview
This project implements a deep learning–based object detection system to identify **crops and weeds** from agricultural field images using **YOLOv8**.  
The solution supports precision agriculture by enabling automated weed detection, which can reduce excessive pesticide usage and improve crop yield.

---

##  Problem Statement
Manual weed detection in large agricultural fields is:
- Time-consuming
- Costly
- Error-prone

This project addresses the problem using **computer vision and deep learning**, automatically detecting crops and weeds from images.

---

##  Solution Approach
- Used **YOLOv8 (You Only Look Once)** for real-time object detection
- Prepared dataset in YOLO annotation format
- Trained the model on agricultural images
- Evaluated performance on validation data
- Visualized predictions with bounding boxes

---

##  Dataset Details
- **Total images:** ~1300  
- **Image size:** 512 × 512 (RGB)  
- **Annotation format:** YOLO  

### Classes
| Class ID | Label |
|--------|-------|
| 0 | Crop |
| 1 | Weed |

---

##  Project Structure

crop-weed-detection/
│
├── data/
│ ├── images/
│ │ ├── train/
│ │ └── val/
│ ├── labels/
│ │ ├── train/
│ │ └── val/
│
├── notebooks/
│ ├── dataset_check.ipynb
│ └── bbox_visualization.ipynb
│
├── data.yaml
├── README.md
└── requirements.txt
Key Learnings
YOLO annotation format and dataset handling
Object detection workflow using YOLOv8
Model training, evaluation, and early stopping
Debugging real-world ML pipeline issues
Performing inference and visualizing results

Applications
Precision agriculture
Automated weed removal systems
Smart farming solutions
Agricultural robotics

 Author
Afisar Alam
Machine Learning Intern

 Project Status
 Completed
 Tested
 Ready for internship submission

