# 🐄 Image-Based Cattle Measurement and Trait Estimation System

An AI-driven computer vision system for automated cattle body measurement and Animal Type Classification (ATC) using image analysis.

---

## 📌 Overview

Manual cattle evaluation is subjective, inconsistent, and not scalable.  
This project provides an automated, image-based system that detects anatomical landmarks, computes body measurements, and generates standardized ATC scores using deep learning.

---

## 🚨 Problem Statement

Traditional livestock assessment:
- Depends on human judgment  
- Prone to bias and fatigue  
- Time-consuming and inconsistent  
- Not suitable for large-scale deployment  

Impact:
- Poor breeding decisions  
- Inaccurate livestock evaluation  
- Lack of standardized data  

---

## 💡 Solution

AI-based pipeline:

<img width="1536" height="500" alt="Pipeline" src="https://github.com/user-attachments/assets/5ddf9774-7e1d-468c-ae7a-2b86803cb3ec" />


- Detect cattle from image  
- Identify anatomical landmarks  
- Compute geometric measurements  
- Normalize ratios  
- Generate standardized ATC score  

---

## ✨ Features

- Automated cattle detection  
- Keypoint-based landmark detection  
- Non-contact body measurement  
- Standardized ATC scoring  
- Works with RGB images (no special hardware)  
- Scalable and field-ready  

---

## 🧠 Methodology

1. **Image Acquisition**  
   - Input: Side-view cattle image  

2. **Animal Detection**  
   - Model: YOLOv8  

3. **Keypoint Detection**  
   - Model: YOLOv8-Pose  

4. **Measurement Extraction**  
   - Distance and angle calculation between keypoints  

5. **Normalization & Scoring**  
   - Ratios computed using withers height  
   - Converted into ATC scores  

---

## 📊 Dataset

- Keypoint-annotated cattle images  
- Real farm conditions  

Variations include:
- Lighting differences  
- Background noise  
- Pose variations  

Link : https://universe.roboflow.com/serhan-0iwep/cow-keypoint-e1ozw/dataset/2

---

## 🛠 Tech Stack

### AI / ML
- YOLOv8  
- YOLOv8-Pose  
- PyTorch  

### Computer Vision
- OpenCV  

### Data Processing
- NumPy  

### Development
- Python  
- Google Colab (training)  
- Gradio (UI)  
- FastAPI (optional backend)  

---

## 🚀 Usage

### Step 1: Upload Image
Provide a side-view cattle image.

<p align="center">
  <img src="https://github.com/user-attachments/assets/e06e3f7c-094e-4940-b4ad-1af19f98d90a" width="45%" />
  <img src="https://github.com/user-attachments/assets/b9bc37f0-bfc4-45c0-bd1f-ca94fe4a1024" width="45%" />
</p>


### Step 2: Processing
The system performs:
- Detection  
- Keypoint extraction  
- Measurement computation


<img width="890" height="670" alt="Screenshot 2026-02-27 001242" src="https://github.com/user-attachments/assets/8d67d377-dc76-431e-8e20-bbf16738a866" />


### Step 3: Output
- Body measurements  
- Trait values  
- Final ATC score  

<p align="center">
  <img src="https://github.com/user-attachments/assets/18fe13fd-f7b6-4f53-95a2-b8d0c6e47530" width="45%" />
  <img src="https://github.com/user-attachments/assets/143fc8b4-5a54-4e76-a50d-2c1ae3a8cf3f" width="45%" />
</p>

For best results:
- Use a well-lit image  
- Avoid heavy glare or obstruction

---

## 🎯 Further Development Goals

- 📈 Expand dataset with diverse cattle breeds and real-world farm conditions  
- 🔍 Improve keypoint detection accuracy under occlusion and complex poses  
- 🧠 Enhance ATC scoring using learned models instead of rule-based ratios  
- 📱 Optimize system for mobile and edge device deployment  
- 🔄 Enable multi-animal detection and tracking in a single frame  
- 💡 Improve robustness against lighting and background variations  
- 🏛 Integrate with livestock management and government databases  

---

## 📊 Expected Results

- Accurate detection of cattle anatomical landmarks  
- Reliable body measurement estimation from images  
- Consistent and unbiased ATC scoring  
- Real-time or near real-time inference capability  
- Scalable and cost-effective livestock evaluation system  

---

## 🤝 Contributing

Contributions are welcome.

- 💡 Suggest improvements  
- 📈 Enhance model accuracy and performance  
- 🔗 Improve scoring methodology  
- ⚙ Optimize deployment and inference speed  

Please ensure:
- Code is clean and modular  
- No sensitive data or credentials are exposed  
- Clear and concise description of changes is included  

---

## 📚 License

This project is developed for academic and research purposes.
