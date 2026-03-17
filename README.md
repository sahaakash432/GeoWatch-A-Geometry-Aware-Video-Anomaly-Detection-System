📌 GeoWatch: Geometry-Aware Video Anomaly Detection

GeoWatch is a computer vision project that combines deep learning + geometric reasoning to improve video anomaly detection.

Instead of relying only on model confidence, it uses real-world spatial constraints (via homography) to make more reliable decisions.

🚀 Pipeline
Video → Detection (YOLOv8) → Tracking → Homography Mapping
      → I3D Classification → Geometric Validation → Anomaly
🧠 Key Ideas

I3D for spatiotemporal action recognition

YOLOv8 + tracking for person localization

Homography to estimate real-world position & speed

Geometry-aware filtering to reduce false positives

📊 Results

~85% validation accuracy (small dataset)

Geometry helps reduce false positives, especially near image edges

⚠️ Limitations

Small custom dataset

Manual calibration

Multi-camera (epipolar) not fully integrated

🔮 Future Work

Larger dataset

Automatic calibration

Multi-camera setup

Newer video models (e.g., SlowFast, Video Swin)
