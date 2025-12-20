# 👁️ See The World Through AI: End-to-End Object Detection

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![YOLOv8](https://img.shields.io/badge/Model-YOLOv8-green)
![Streamlit](https://img.shields.io/badge/Framework-Streamlit-red)
![OpenCV](https://img.shields.io/badge/Library-OpenCV-yellow)

A comprehensive Computer Vision project exploring object detection using **Ultralytics YOLOv8**. This project documents a 5-day journey ranging from running inference on static images to training custom models and deploying a full-stack web application using Streamlit and Ngrok.



## 🚀 Project Overview

This repository contains code and resources for:
1.  **Static Image Detection:** Identifying objects in uploaded photos.
2.  **Video Analysis:** Frame-by-frame detection on video files.
3.  **Real-time Inference:** capturing snapshots via webcam integration in Google Colab.
4.  **Custom Training:** Fine-tuning YOLOv8n on the COCO128 dataset.
5.  **Web Deployment:** An interactive GUI built with Streamlit for easy user interaction.

## 📂 Project Structure (Day-by-Day)

### Day 1: Setup & Image Detection
* **Goal:** Environment setup and "Hello World" of Object Detection.
* **Tech:** Installed `ultralytics`, `opencv-headless`, `matplotlib`.
* **Outcome:** Successfully loaded the pretrained `yolov8n.pt` model and detected objects (persons, chairs, laptops) in a test image.

### Day 2: Object Detection on Video
* **Goal:** Processing moving visuals.
* **Process:** * Loaded a video file (`Kota_prism.mp4`).
    * Processed the video frame-by-frame.
    * Applied YOLO inference and annotated frames.
* **Outcome:** Generated `output_detected.mp4` with bounding boxes around kites, cars, and traffic lights.

### Day 3: Webcam Snapshot Integration
* **Goal:** Interactive input within a notebook environment.
* **Process:** Utilized JavaScript injection to access the local webcam within Google Colab, captured a `snapshot.jpg`, and ran immediate inference.

### Day 4: Mini YOLO Training
* **Goal:** Understanding the training pipeline.
* **Dataset:** COCO128 (Small dataset for rapid prototyping).
* **Config:** Custom `data.yaml` defining 80 classes.
* **Training:** Trained `yolov8n.pt` for 10 epochs.
* **Results:** Achieved a mAP50 of ~0.69 after just 10 epochs.
* **Artifacts:** Custom weights saved as `best.pt`.

### Day 5: Deployment with Streamlit
* **Goal:** Creating a user-friendly interface.
* **App Features:**
    * Upload Image or Video.
    * Upload Custom Weights (`.pt`).
    * Adjust Confidence Threshold via slider.
    * Select Inference Image Size.
* **Hosting:** Exposed the local Streamlit server to the web using **Ngrok**.



## 🛠️ Installation & Usage

### Prerequisites
* Python 3.8+
* Google Colab (Recommended for GPU training)

### Dependencies
Create a `requirements.txt` file with the following:
```text
ultralytics==8.3.0
streamlit==1.38.0
pyngrok==7.1.6
opencv-python-headless
pillow
pandas
matplotlib

```

### Running the App (Colab/Local)

To run the Streamlit app specifically:

1. **Install requirements:**
```bash
pip install -r requirements.txt

```


2. **Run the app:**
```bash
streamlit run app_streamlit.py

```


3. **Expose via Ngrok (if running in Colab):**
```python
from pyngrok import ngrok
public_url = ngrok.connect(8501)
print(public_url)

```



## 📊 Model Performance (Day 4 Training)

Training was performed on the COCO128 dataset for 10 epochs.

| Metric | Value |
| --- | --- |
| **mAP50** | 0.697 |
| **Precision** | 0.674 |
| **Recall** | 0.652 |
| **Inference Speed** | ~2.7ms per image (Tesla T4) |

## 📸 Screenshots

*Placeholder for screenshot of the Streamlit Interface*
*Placeholder for screenshot of a detected image*

## 🤝 Acknowledgments

* **Ultralytics** for the incredible YOLOv8 library.
* **Streamlit** for the rapid application development framework.
* **Google Colab** for providing free GPU resources.

---

*Created by Aayush*

```

### Next Step
Would you like me to generate the specific **`requirements.txt`** file or help you write the code to create a specific **visual diagram** for the architecture section?

```
