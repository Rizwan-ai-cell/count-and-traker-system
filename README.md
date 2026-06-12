# Count and Tracker System

Simple people counting and tracking demo using Ultralytics YOLO and OpenCV.

## Overview

This project detects and tracks people in a video, counting entries and exits across two polygonal areas.

## Requirements

- Python 3.8+
- pip packages: `ultralytics`, `opencv-python`, `pandas`, `numpy`
- A YOLOv8 model file (this repo includes `yolov8s.pt`)
- A video file (update the path in `main.py`, default: `peoplecount1.mp4`)

Install Python dependencies:

```bash
pip install ultralytics opencv-python pandas numpy
```

## Usage

1. Make sure `yolov8s.pt` is present in the project root (already included).
2. Place your input video in the project root or update the path in `main.py`.
3. Run:

```bash
python3 main.py
```

While running, the script will open a window named `RGB` showing detections and counts. Press `Esc` to exit.

## Notes

- The `tracker.py` implements a simple centroid tracker.
- The shapes `area1` and `area2` are defined in `main.py`; adjust coordinates as needed for your video.
- The repository currently includes a large model file (`yolov8s.pt`). If you already have a model installed elsewhere, update `main.py` to load that path.

## License

No license specified. Check the original author's repository for licensing details.
