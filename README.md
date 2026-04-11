# 🛡️ Face Liveness Detection System

A real-time face liveness detection system that distinguishes between **live (real)** faces and **spoofed (fake)** faces such as photos or videos.  
Built using **YOLOv8 (Ultralytics)**, this project enhances security in face recognition systems by preventing spoofing attacks.

---

## 🚀 Features

- Real-time face detection using webcam  
- Deep learning-based classification (Real vs Fake)  
- Fast inference with YOLOv8  
- Confidence score display  
- Complete pipeline: data collection → training → deployment  

---

## 🧠 Model Details

- Model: YOLOv8  
- Classes: `Real`, `Fake`  
- Framework: PyTorch  
- Input Size: 640×640  
- Dataset: Custom collected dataset  

---

## 📂 Project Structure
```

Face-Liveness-Detection/
│
├── main.py
├── train.py
├── splitData.py
├── dataCollection.py
│
├── Dataset/
│   └── SplitData/
│       └── dataOffline.yaml
│
├── Testing Scripts/
│   ├── yoloTest.py
│   └── faceDetectorTest.py
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation
```

git clone https://github.com/aadeshyogi12/Face-Liveness-Detection.git  
cd Face-Liveness-Detection  
pip install -r requirements.txt  
```

If requirements.txt is not available:
```

pip install opencv-python cvzone ultralytics  
```

---

## ▶️ Usage

### 1. Data Collection

Edit class ID in dataCollection.py:

classID = 0  # 0 = Fake, 1 = Real  

Run:
```

python dataCollection.py  
```

---

### 2. Split Dataset
```

python splitData.py  
```

---

### 3. Train Model
```

python train.py  
```

---

### 4. Run Real-Time Detection
```

python main.py  
```

---

## 🧪 Output

- REAL → Live face detected  
- FAKE → Spoof detected  
- Confidence score displayed  

---

## 🛠️ Tech Stack

- Python  
- OpenCV  
- CVZone  
- Ultralytics YOLOv8  
- PyTorch  

---

## ⚠️ Limitations

- Performance may drop in low light  
- Requires diverse dataset for better accuracy  
- Limited against advanced spoofing (e.g., deepfakes, 3D masks)  

---
