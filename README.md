# Knowledge-Distilled YOLOv11 for Structural Crack Detection
Lightweight and real-time crack detection model using a YOLOv11 Teacher–Student framework with Pseudo-Labeling and Knowledge Distillation.  
Designed for structural health monitoring, surface flaw localization, and automated inspection in construction environments.

---

## 🚀 Features
✅ YOLOv11-L (Teacher) → YOLOv11-N (Student) knowledge transfer  
✅ Pseudo-labeling for unlabeled or low-quality annotations  
✅ Faster inference with near-teacher accuracy  
✅ Works on asphalt, concrete, plaster, and mixed wall surfaces  
✅ Augmentation pipeline integrated for robustness (rotation, exposure, grayscale, crop, etc.)

---

## 📁 Dataset
Images include crack samples under different lighting, material textures, and orientations.  
Bounding boxes are provided in YOLO format.  
If the dataset is public, add the link here:
- Dataset Source: [Roboflow / Custom Annotated Dataset](https://app.roboflow.com/computer-vision-yqyos/merged-cracks/3)
- Image count: 11,046 (with augmentation)

---

## 🧠 Model Architecture
- Base: YOLOv11-N / YOLOv11-L (Ultralytics)
- Anchor-free detection
- KD + pseudo-label pipeline
- Loss terms: Regression, Class, DFL, KD-weighted terms

## Dataset
https://app.roboflow.com/computer-vision-yqyos/merged-cracks/

Student gains:
- Lower computational cost
- Faster inference
- Comparable metric performance to teacher model

---

## 🔧 Installation
```bash
git clone https://github.com/USER/REPO.git
cd REPO
pip install -r requirements.txt
