# YOLO-AR-Android

🚀 An offline **Android Augmented Reality (AR) app** that uses a quantized **YOLO ONNX model** for real-time object detection and overlays AR elements on detected objects.  

This project integrates:
- **ONNX Runtime (Mobile)** → run YOLO model on-device
- **CameraX API** → real-time camera frames
- **ARCore / Sceneform** → AR overlays
- **Kotlin + Gradle** → Android native development

---

## 📌 Features
- 🔋 Fully **offline** (no Roboflow API, no internet needed)
- ⚡ Runs **quantized YOLO ONNX model** for efficiency
- 🎥 Real-time detection on camera feed
- 🌍 AR overlays (bounding boxes, labels, or 3D objects)
- 📱 Android-native, works on most modern phones

---

## 📂 Project Structure
```

YOLO-AR-Android/
│── app/
│   ├── src/main/java/com/example/yoloar/
│   │   ├── MainActivity.kt      # Camera + AR entry point
│   │   ├── YoloDetector.kt      # ONNX Runtime inference
│   │   ├── AROverlay.kt         # AR visualization
│   │   └── Utils.kt             # Pre/post processing
│   ├── src/main/res/            # UI layouts, icons
│   └── src/main/assets/
│       └── yolo.onnx            # Quantized YOLO model
│
├── README.md
├── build.gradle
└── .github/workflows/android.yml   # GitHub Actions → build APK

````

---

## ⚙️ Setup & Run

### 1. Clone Repo
```bash
git clone https://github.com/<your-username>/YOLO-AR-Android.git
cd YOLO-AR-Android
````

### 2. Add Model

Place your quantized YOLO model (`yolo.onnx`) inside:

```
app/src/main/assets/
```

### 3. Build with GitHub Actions

* Push your changes → GitHub Actions builds the APK automatically
* Download the generated APK from **Actions → Artifacts**

### 4. Install on Android

* Transfer APK to your device
* Enable *Install from Unknown Sources*
* Install & run 🚀

---

## 📜 License

MIT License – free to use, modify, and share.

---

## 🤝 Contributing

PRs and feature suggestions are welcome. Open an issue to start the discussion!

---
