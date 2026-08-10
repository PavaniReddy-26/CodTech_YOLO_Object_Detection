# YOLO Object Detection App

-  Real-time object detection (YOLO11)
-  Upload image or video easily (drag & drop)
-  Choose model type: Fast / Balanced / Accurate
-  Smart streaming for video results
-  Dark mode styled UI
-  Reset and upload new file anytime

---

## Getting Started

1. **Clone this repo**
   ```bash
   git clone https://github.com/PavaniReddy-26/CodTech_YOLO_Object_Detection

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Download YOLO models**
   Put your models (e.g. `yolo11n.pt`) in the `models/` directory.
   Get them from:
   [Ultralytics Official Models](https://docs.ultralytics.com/models)

4. **Run the app**

   ```bash
   uvicorn app.main:app --reload
   ```

5. Open `http://127.0.0.1:8000` in your browser.

---

## Project Structure

```
YOLO-Object-Detection-App/
├── app/                # FastAPI backend
│   ├── image_processor.py
│   ├── main.py
│   ├── model_loader.py
│   └── stream_processor.py
├── static/             # Frontend JS/CSS
│   ├── script.js
│   └── style.css
├── templates/          # HTML template
│   └── index.html
├── models/             # YOLO .pt models
│   ├── yolo11m
│   ├── yolo11n
│   └── yolo11s
├── requirements.txt
└── README.md
```

---

## Tech Stack

* **FastAPI** – lightweight Python backend
* **Ultralytics YOLO** – object detection engine
* **JavaScript + HTML + CSS** – frontend
* **Font Awesome** – icons

---
py -3.12 --version
py -3.12 -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
python -m uvicorn app.main:app --reload
