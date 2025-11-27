# 🤖 AI-Jaga You Lah
* AI Patient Severity Monitor which is a Computer-Vision–Powered Triage Assistant for Hospital Waiting Areas*

## AI in Medicine Summer School 2025 Mini Project

Team Members:
- Chang Yong Qi
- Lai Ai Ling
- Toh Ka Peng
- Yong Yi Shean
- Hor Yee Min

---

## 🩺 **Overview**
Incidents of patients collapsing or becoming critically ill in hospital waiting rooms have been increasingly reported. Overcrowding, long waiting times, and unnoticed patient deterioration can lead to severe consequences — including death.

This project, **AI Patient Severity Monitor**, aims to assist hospitals by automatically assessing patient severity levels through **pose detection** and **facial expression analysis** while they are waiting to see a doctor.

The system continuously monitors patients using a camera and identifies critical conditions such as:
- Slouching posture (weakness)
- Holding chest / leaning forward (pain)
- Unconscious posture
- Distress or severe discomfort facial expressions

If detected, the system can alert staff — potentially saving lives.

---

## 🎯 **Objectives**
- Detect abnormal or concerning patient postures
- Classify severity level (Normal, Moderate Distress, High Severity)
- Provide real-time predictions from webcam input
- Deploy as a simple web-based AI system at hospital counters or waiting areas

---

## 💡 **Features**
- ✔ Real-time pose detection using Teachable Machine Pose Model  
- ✔ Automatic severity classification (custom-trained model)  
- ✔ Facial expression + body posture possibility  
- ✔ Mobile and desktop camera switching  
- ✔ Confidence-level color indicators  
- ✔ Camera permission error handling  
- ✔ Clean, responsive UI

---

## 🏗️ **System Architecture**
Camera → Pose Model (Teachable Machine + TensorFlow.js)
- Classification Layer
- Severity Level Output
- (Optional) Alert System / Monitoring Dashboard

---

## 📦 **Tech Stack**
| Component | Technology |
|----------|------------|
| **Frontend** | HTML, CSS, JS |
| **AI Model** | Teachable Machine (Pose Classification) |
| **AI Framework** | TensorFlow.js |
| **Deployment** | Static Web Server / GitHub Pages / VSCode Live Server |

---

## 📊 Dataset Preparation

Since no public dataset exists for patient severity posture, the team collected and labeled the data manually.

### **📁 Dataset Sources**
1. **Internet images** (patients fainting, dizziness, chest pain, etc.)  
2. **Acted pictures** by team members  

### **📌 Labels**
Common severity categories:
- `Normal`
- `Mild Discomfort`
- `Moderate Pain`
- `High Severity (Risk)`
- `Unconscious / Collapse`

### **📷 Data Requirements**
- Minimum **200 images per class**  
- More data = better accuracy  
- Mix of:
  - Different body angles  
  - Sitting vs standing  
  - Different lighting  
  - Different genders & physiques  

### **🖼️ Tools Used**
- Teachable Machine (Pose Model)
- Roboflow (optional)
- Manual labeling

---

## 🤖 Model Training

### **1. Train Pose Model**
Use **Teachable Machine: Pose Classification**  
Add classes → Upload training images → Train → Export model

### **2. Export Model**
Download the **model folder**:
