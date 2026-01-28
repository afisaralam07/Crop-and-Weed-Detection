#  Crop & Weed Detection using YOLOv8

##  Project Overview
This project implements a deep learning–based **object detection system** to identify **crops and weeds** from agricultural field images using **YOLOv8**.  
The solution supports **precision agriculture** by enabling automated weed detection, helping reduce excessive pesticide usage and improve crop yield.

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
- Prepared dataset in **YOLO annotation format**  
- Trained the model on agricultural images  
- Evaluated performance on validation data  
- Visualized predictions using bounding boxes  

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

Perfect 
Main tumhara README final, internship-ready bana raha hoon.
Isme kya add karna hai, kya hatana hai — sab already fix hai.

Tumhe bas poora content copy–paste karna hai
Kuchh bhi sochna ya edit nahi karna

 FINAL README.md (COPY–PASTE THIS EXACTLY)
#  Crop & Weed Detection using YOLOv8

##  Project Overview
This project implements a deep learning–based **object detection system** to identify **crops and weeds** from agricultural field images using **YOLOv8**.  
The solution supports **precision agriculture** by enabling automated weed detection, helping reduce excessive pesticide usage and improve crop yield.

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
- Prepared dataset in **YOLO annotation format**  
- Trained the model on agricultural images  
- Evaluated performance on validation data  
- Visualized predictions using bounding boxes  

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


---

##  Model & Training Details
- **Model:** YOLOv8n  
- **Framework:** Ultralytics YOLOv8  
- **Image Size:** 512 × 512  
- **Epochs Trained:** 17 (early stopping after convergence)  
- **Hardware:** CPU  

Training was stopped early after observing stable loss values to avoid overfitting and reduce computation cost.

---

## Evaluation Results
| Metric | Value |
|------|------|
| Precision | ~0.81 |
| Recall | ~0.71 |
| mAP@50 | ~0.81 |
| mAP@50–95 | ~0.49 |

The model successfully detects multiple crops and weeds per image with good accuracy.

---

## Inference & Results
- **Inference speed:** ~70 ms per image (CPU)  
- **Bounding boxes:**
  - Green → Crop  
  - Red → Weed  

Prediction results are saved in:


---

##  How to Run the Project

###  Install Dependencies
```bash
pip install ultralytics opencv-python matplotlib

### Train the Model
yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=50 imgsz=512 batch=8

### Run Inference
yolo task=detect mode=predict model=best.pt source=data/images/val

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

