# Object_IQ 🚀

**Advanced Real-Time Object Detection & Intelligence System**

A powerful YOLOv8-based surveillance system with DeepSORT tracking, crowd analytics, weapon detection, and live web dashboard.

---

## ✨ Features

- Real-time Object Detection (YOLOv8)
- DeepSORT Multi-Object Tracking
- Crowd Counting + Heatmap
- Weapon/Suspicious Object Detection
- Live Web Dashboard
- MongoDB Atlas Storage
- Email Notifications
- Snapshot Capture
- Hardware (Arduino) Ready

---

## 🚀 How to Run on Your Local System (After Cloning)

### Step-by-Step Guide:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/CsWithAk/Object_IQ.git
   cd Object_IQ

2. **Create Virtual Environment (Strongly Recommended)**
   ```bash
   python -m venv venv

   # Windows
   venv\Scripts\activate

   # Linux / macOS
   source venv/bin/activate
   
3. Install Dependencies
   ```bash
   pip install -r requirements.txt

4. Configure the Project
	Copy config/config.yaml and update:
	Camera source (0 for webcam)
	MongoDB connection string
	Email credentials (use App Password for Gmail)

	Customize config/objects.yaml as needed.

5. run only Software
   ```bash
   cd src
   python run_dashboard.py

6. run full system (software + hardware)
   ```bash
   cd Hardware
   python run_with_hardware.py
	
7. project Structure



**Dashboard Features**
```bash
Live video feed with detections
Real-time statistics and crowd count
Heatmap visualization
Alert history
Responsive design

**Note:**

A. Configuration Guide

config/config.yaml → General settings, camera, database, email
config/objects.yaml → Target objects & custom rules
  
B. Troubleshooting
    Common Issues:

Camera not opening → Change camera.source to 0 or correct RTSP URL
MongoDB connection failed → Check your connection string
Email not working → Use Gmail App Password (not normal password)
Port already in use → Change dashboard port in run_dashboard.py



**Contributing**
Contributions are welcome! Feel free to open issues or submit pull requests.
