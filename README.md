```
<div align="center">

# 🏋️ Bulgarian Split Squat AI Trainer

<img src="https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/YOLOv11-Pose-red?style=for-the-badge&logo=yolo&logoColor=white"/>
<img src="https://img.shields.io/badge/OpenCV-4.x-green?style=for-the-badge&logo=opencv&logoColor=white"/>
<img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge"/>

<br/>
<br/>

**Real-time AI-powered fitness coach that tracks your Bulgarian Split Squats, counts reps, and corrects your form instantly!**

[Features](#-features) •
[Demo](#-demo) •
[Installation](#-installation) •
[Usage](#-usage) •
[How It Works](#-how-it-works)

<br/>

<img src="https://raw.githubusercontent.com/Amirhosseinzandi-web/BulgarianSquat-Tracker/main/demo.gif" width="600" alt="Demo GIF"/>

</div>

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🎯 **Rep Counter** | Automatically counts your reps with high accuracy |
| 📐 **Form Analysis** | Real-time feedback on your exercise form |
| 🦵 **Auto Leg Detection** | Detects which leg is the working leg |
| 📊 **Depth Tracking** | Visual depth bar shows how deep you're squatting |
| 🏆 **Scoring System** | Get scored on each rep (Perfect = 100 pts) |
| ⚙️ **Adjustable Difficulty** | Make it easier or harder with +/- keys |

---

## 🔍 Form Checks

The AI monitors these common mistakes:

❌ KEEP CHEST UP → Torso leaning too far forward
❌ LEVEL YOUR HIPS → Hips are uneven/tilted
❌ GO DEEPER → Not hitting proper depth

When your form is perfect: ✅ PERFECT FORM

---

## 🚀 Installation

### Prerequisites

- Python 3.8 or higher
- Webcam

### Setup

Clone the repository:
git clone https://github.com/Amirhosseinzandi-web/BulgarianSquat-Tracker.git
cd BulgarianSquat-Tracker

Install dependencies:
pip install ultralytics opencv-python numpy

Run the application:
python app.py

---

## 🎮 Usage

### Controls

| Key | Action |
|-----|--------|
| Q | Quit application |
| R | Reset stats |
| + | Make exercise easier |
| - | Make exercise harder |

### Tips for Best Results

1. 📷 **Camera Position**: Place camera to your side (profile view)
2. 💡 **Lighting**: Ensure good lighting for accurate detection
3. 📏 **Distance**: Stand 2-3 meters from camera
4. 👕 **Clothing**: Wear fitted clothes for better keypoint detection

---

## 🧠 How It Works

┌─────────────┐     ┌──────────────┐     ┌─────────────┐
│   Webcam    │ ──► │  YOLOv11     │ ──► │   Angle     │
│   Input     │     │  Pose Est.   │     │   Calc      │
└─────────────┘     └──────────────┘     └──────────────┘
                                                │
                                                ▼
┌─────────────┐     ┌──────────────┐     ┌─────────────┐
│   Display   │ ◄── │    Form      │ ◄── │   State     │
│   Output    │     │    Check     │     │   Machine   │
└─────────────┘     └──────────────┘     └─────────────┘

### Key Components

- **Pose Estimation**: YOLOv11n-pose for real-time keypoint detection
- **Angle Calculation**: 3-point angle calculation at knee joint
- **State Machine**: UP → DOWN → UP cycle for rep counting
- **Form Analysis**: Torso lean, hip balance, and depth checks

---

## 📊 Scoring System

| Score | Meaning |
|-------|---------|
| 💯 **100** | Perfect rep - no form errors |
| 🔶 **70** | Rep completed with form errors |

Average score is displayed at the bottom of the screen.

---

## 🛠️ Tech Stack

<div align="center">

| Technology | Purpose |
|------------|---------|
| ![Python](https://img.shields.io/badge/Python-FFD43B?style=flat-square&logo=python&logoColor=blue) | Core Language |
| ![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=flat-square&logo=OpenCV&logoColor=white) | Video Processing |
| ![YOLO](https://img.shields.io/badge/YOLOv11-00FFFF?style=flat-square&logo=yolo&logoColor=black) | Pose Estimation |
| ![NumPy](https://img.shields.io/badge/Numpy-777BB4?style=flat-square&logo=numpy&logoColor=white) | Calculations |

</div>

---

## 📁 Project Structure

BulgarianSquat-Tracker/
├── 📄 app.py              # Main application
├── 📄 app.ipynb           # Jupyter notebook version
├── 📄 requirements.txt    # Dependencies
├── 📄 README.md           # This file
└── 🎥 demo.gif            # Demo animation

---

## 🔮 Future Improvements

- [ ] 🏃 Add more exercises (Lunges, Squats, Deadlifts)
- [ ] 📱 Mobile app version
- [ ] 📈 Progress tracking & history
- [ ] 🔊 Voice feedback
- [ ] 🎵 Workout music integration

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (git checkout -b feature/AmazingFeature)
3. Commit changes (git commit -m 'Add AmazingFeature')
4. Push to branch (git push origin feature/AmazingFeature)
5. Open a Pull Request

---

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

<div align="center">

### ⭐ Star this repo if you found it helpful!

<br/>

Made with ❤️ by [Amir Hossein Zandi](https://github.com/Amirhosseinzandi-web)

<br/>

<img src="https://img.shields.io/github/stars/Amirhosseinzandi-web/BulgarianSquat-Tracker?style=social"/>
<img src="https://img.shields.io/github/forks/Amirhosseinzandi-web/BulgarianSquat-Tracker?style=social"/>

</div>
```
