# ✋ Real-Time Hand Sign Recognition

A **real-time hand sign recognition system** built with **Python, OpenCV, and cvzone**.  
The project uses a **custom-trained Keras model** (via Teachable Machine) to classify hand gestures into **A, B, and C**.  

---

## 🚀 Features
- Detects and tracks a single hand using **cvzone HandTrackingModule**  
- Crops and preprocesses the hand image into a **300×300 white canvas** for consistent model input  
- Classifies hand gestures with a **custom-trained Teachable Machine Keras model (`keras_model.h5`)**  
- Displays prediction labels and bounding boxes in **real-time via webcam**  
- Built as a **learning project** to explore computer vision and deep learning  

---

## 🛠️ Tech Stack
- **Python**  
- **OpenCV** – real-time image capture and processing  
- **cvzone** – hand detection and preprocessing utilities  
- **TensorFlow/Keras** – model training and classification  
- **NumPy, Math** – data manipulation  

---

## 📂 How It Works
1. A webcam feed is captured in real-time.  
2. The hand is detected and cropped with a margin (`offset`).  
3. The cropped image is resized and placed on a **300×300 white background**.  
4. The preprocessed image is fed into the **Keras model** trained on hand signs A, B, and C.  
5. Predictions are displayed on the webcam feed with labels and bounding boxes.  

---

## ▶️ Usage

Install dependencies:
```bash
pip install opencv-python cvzone tensorflow numpy
