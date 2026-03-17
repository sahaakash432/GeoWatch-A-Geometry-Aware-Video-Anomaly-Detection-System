# 📌 GeoWatch: Geometry-Aware Video Anomaly Detection

## 📖 Overview

GeoWatch is a computer vision project that combines deep learning and geometric reasoning to improve video anomaly detection.

Instead of relying only on model confidence, it incorporates real-world spatial constraints using homography, enabling more reliable and context-aware anomaly detection.

---

## 🚀 Pipeline

```
Video → Detection (YOLOv8) → Tracking → Homography Mapping
      → I3D Classification → Geometric Validation → Anomaly
```

---

## 🧠 Key Ideas

* **I3D** for spatiotemporal action recognition
* **YOLOv8 + tracking** for accurate person localization
* **Homography mapping** to estimate real-world position and speed
* **Geometry-aware filtering** to reduce false positives

---

## 📊 Results

* ~85% validation accuracy (on a small dataset)
* Geometry-based reasoning helps reduce false positives, especially near image boundaries

---

## ⚠️ Limitations

* Small custom dataset
* Manual camera calibration required
* Multi-camera setup (epipolar geometry) not fully implemented

---

## 🔮 Future Work

* Expand dataset size and diversity
* Automate camera calibration
* Integrate multi-camera system
* Explore advanced video models (e.g., SlowFast, Video Swin)

---

## 🛠️ Technologies Used

* Python
* PyTorch
* OpenCV
* YOLOv8
* I3D (Inflated 3D ConvNet)

---

## ▶️ Usage

1. Clone the repository:

```
git clone https://github.com/your-username/geowatch.git
```

2. Navigate to the project directory:

```
cd geowatch
```

3. Install dependencies:

```
pip install -r requirements.txt
```

4. Run the pipeline:

```
python main.py
```

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---
