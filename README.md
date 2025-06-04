# Automatic License Plate Recognition (ALPR)

## 📄 Abstract
This project implements an end-to-end **Automatic License Plate Recognition (ALPR)** system using deep learning and optical character recognition (OCR). The primary objective is to accurately detect and recognize vehicle license plates from images in real-time. The system leverages **YOLOv8** (You Only Look Once, Version 8) for license plate detection and integrates **EasyOCR** and **Pytesseract** for character recognition.

A custom dataset was constructed using both publicly available vehicle images and user-captured photographs under varying environmental conditions. All annotations were converted from Pascal VOC to YOLO format to ensure compatibility with the YOLOv8 training pipeline. The model was trained with extensive preprocessing and augmentation techniques to improve generalization.

The results indicate that the system performs robustly across different image conditions, achieving high detection accuracy and satisfactory text recognition. Although OCR misclassification was observed in cases of motion blur and stylized fonts, the system proves effective for use in traffic monitoring, law enforcement, and toll management systems.

---

## 🚀 Features
- License plate detection using YOLOv8
- Optical character recognition using EasyOCR and Pytesseract
- Preprocessing: grayscale conversion, noise reduction, CLAHE, thresholding
- Post-processing: text cleanup and correction
- Exportable results with bounding boxes and plate text

---

## 📁 Dataset
- Public ALPR datasets + custom-captured images
- Converted annotations from Pascal VOC to YOLO format
- Includes varied lighting, angles, and motion blur scenarios

---

## 🛠️ Models Used
- **YOLOv8**: Real-time object detection
- **EasyOCR / Pytesseract**: OCR engines for license plate text recognition

---

## 📊 Performance Metrics
- **Precision 100**
- **Recall 70**
- **F1-Score 82**
- **mAP@0.5, mAP@0.5:0.95** for YOLOv8


## 📌 Future Enhancements
- Multilingual plate recognition
- Real-time edge deployment (Jetson Nano, Raspberry Pi)
- Improved OCR using transformer-based text recognition
