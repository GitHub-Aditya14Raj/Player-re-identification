
# 🏃‍♂️ Player Re-Identification in Sports Footage

This project solves the real-world problem of **tracking football players** in a 15-second video using a pre-trained YOLO model and **appearance-based re-identification**. The system ensures that each player keeps a consistent ID throughout the video, even after temporarily going out of view.

---

## 🎯 Objective

To implement a robust computer vision pipeline that:
- Detects players in a football match video using a custom-trained YOLOv5 model.
- Assigns a unique ID to each player.
- Maintains consistent IDs across frames using spatial and visual appearance matching.
- Outputs a new video showing player bounding boxes with re-identified IDs.

---

## 🧠 Model

The object detection model `best.pt` (YOLOv5, fine-tuned for players and the ball) is too large to upload directly to GitHub.

📥 **Download it here:**  
🔗 [Download best.pt from Google Drive](https://drive.google.com/file/d/1nXDMKv3TDELz2zyKZZtcC4Off0K_g0_Q/view?usp=sharing)

After downloading:
- Place `best.pt` in the same directory as the notebook before running.

---

## 📁 Files Included

- `main.ipynb` — Complete pipeline with detection, tracking, and video generation.
- `15sec_input_720p.mp4` — Input match footage (15 seconds).
- `output.mp4` — Output video with bounding boxes and consistent player IDs.
- `README.md` — This file.

---

## ⚙️ Dependencies & Environment

Tested on: **Google Colab / Python 3.10**

### 📦 Required Libraries

Install these via pip if running locally:

```bash
pip install ultralytics opencv-python torch torchvision scipy tqdm
```


🚀 How to Run

1)Open main.ipynb in Google Colab (recommended) or your local environment.

2)Download the YOLO model (best.pt) from the Google Drive link above.

3)Upload these files to your runtime:

best.pt

15sec_input_720p.mp4

4)Run the notebook cells.

It will produce output.mp4 with real-time player re-identification and tracking.


