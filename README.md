
---

# Team Gestura 🤟 – ASL Gesture Detection

**Breaking Barriers, One Gesture at a Time**

---

## Table of Contents

* [Overview](#overview)
* [Features](#features)
* [Demo](#demo)
* [Installation](#installation)
* [Usage](#usage)
* [Configuration](#configuration)
* [Supported Input Modes](#supported-input-modes)
* [Voice Feedback](#voice-feedback)
* [Contributing](#contributing)
* [License](#license)

---

## Overview

**Team Gestura** is a web-based application for **real-time ASL (American Sign Language) gesture detection** built with:

* **Python**
* **RPi 3B** for the processing
* **YOLOv8** for gesture detection
* **OpenCV** for image/video processing

It allows users to detect hand gestures from a **webcam, uploaded images, or videos** and provides **voice feedback** using browser-based speech synthesis.

The app is designed to make **communication with the hearing-impaired easier** and to serve as a **practical demonstration of AI-based gesture recognition**.

---

## Features

* **Real-time ASL gesture detection** using YOLOv8
* **Multiple input modes:** webcam, image upload, video upload
* **Dashboard:** displays average FPS, total gestures detected, and model confidence
* **Voice feedback:** automatically announces detected gestures (via browser speech synthesis)
* **User feedback form:** allows users to rate and leave comments about the app
* Fully **web-based**, compatible with **Streamlit Cloud**

---

## Installation

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/Gestura-RPI_code
cd gestura-app
```

2. **Create a virtual environment**

```bash
python -m venv venv
source venv/bin/activate   # Linux
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Download the trained YOLOv8 model** (`best.pt') and place it in the project root.

---

## Usage

1. **Run locally**

```bash
python3 main.py
```
python main.py --model=yolo11n_ncnn_model --source=usb0 --resolution=640x480

4. **Adjust settings**:

   * Confidence threshold
   * Enable/disable voice feedback


---


## Supported Input Modes

* **Webcam:** Capture gestures in real-time (local webcam or browser camera)
* **Image:** Upload an image and detect gestures
* **Video:** Upload a video file for frame-by-frame gesture detection

---

## Voice Feedback

* Uses **browser-based speech synthesis** on Streamlit Cloud.
* Automatically announces detected gestures when enabled.
* Local users (Linux) can optionally use `espeak` if desired.

---

## Contributing

Contributions are welcome! You can:

* Improve gesture detection
* Add new ASL gestures
* Enhance the UI or dashboard
* Fix bugs or optimize performance

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

---

## License

This project is a open source anybody can acess and develop it for their personal needs.

---

**Team Gestura 💙 – Breaking barriers, one gesture at a time!**

---

