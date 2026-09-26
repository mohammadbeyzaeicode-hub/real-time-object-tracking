# Real-Time Object Detection & Tracking

A computer vision project for building a real-time system that detects, tracks, and analyzes objects in video streams.

The project is being developed incrementally, starting from object detection and moving toward multi-object tracking, trajectory analysis, object counting, and system evaluation.

## Project Goal

Build a practical computer vision pipeline that can:

* Detect objects in images and video
* Track objects across consecutive frames
* Maintain persistent object identities
* Extract object trajectories
* Count objects based on their movement
* Evaluate detection and tracking performance
* Analyze failure cases and robustness

## Current Pipeline

```text
Video
  ↓
YOLO Object Detection
  ↓
Bounding Boxes + Classes + Confidence
  ↓
ByteTrack
  ↓
Track IDs
  ↓
Trajectory Analysis
  ↓
Counting
  ↓
Evaluation
```

## Current Progress

### Completed

* [x] YOLO object detection baseline
* [x] Detection output analysis
* [x] IoU implementation and analysis
* [x] Non-Maximum Suppression (NMS)
* [x] Class-aware NMS
* [x] Video-based object detection
* [x] Detection processing FPS measurement
* [x] Basic IoU-based tracking concept
* [x] YOLO + ByteTrack integration
* [x] Track ID visualization

### In Progress

* [ ] Object trajectory extraction
* [ ] Trajectory visualization
* [ ] Object counting
* [ ] Tracking evaluation
* [ ] Robustness and failure analysis
* [ ] Final real-time demo

## Project Structure

```text
real-time-object-detection-tracking/
│
├── notebooks/
│   ├── 01_yolo_baseline.ipynb
│   ├── 02_detection_analysis.ipynb
│   ├── 03_video_detection.ipynb
│   └── 04_object_tracking.ipynb
│
├── src/
│   ├── detection/
│   ├── tracking/
│   ├── evaluation/
│   └── visualization/
│
├── experiments/
├── demo/
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Notebooks

The notebooks are used as an experimental and learning environment.

### `01_yolo_baseline.ipynb`

Initial exploration of YOLO object detection.

Topics:

* Object classes
* Bounding boxes
* Confidence scores
* Detection results

### `02_detection_analysis.ipynb`

Analysis of fundamental detection concepts.

Topics:

* Intersection over Union (IoU)
* Non-Maximum Suppression (NMS)
* Class-aware NMS
* Detection filtering

### `03_video_detection.ipynb`

Extends object detection from images to video.

Topics:

* Frame-by-frame processing
* Video input/output
* Detection visualization
* Processing FPS

### `04_object_tracking.ipynb`

Extends the detection pipeline with multi-object tracking.

Topics:

* Detection vs. tracking
* IoU-based matching
* Track IDs
* Simple tracking concepts
* ByteTrack integration

## Technologies

* Python
* PyTorch
* Ultralytics YOLO
* OpenCV
* ByteTrack
* Jupyter / Google Colab

## Development Approach

The project separates experimentation from the main implementation.

**Notebooks** are used to:

* Understand computer vision concepts
* Test ideas
* Run experiments
* Analyze results

The `src/` directory is intended for reusable project code.

As the project evolves, validated experiments will be converted into reusable modules.

## Roadmap

```text
[x] Object Detection
[x] Video Detection
[x] Object Tracking
[ ] Trajectory Analysis
[ ] Object Counting
[ ] Tracking Evaluation
[ ] Robustness Analysis
[ ] Final Demo
```

## Collaboration

The project is intended to be developed collaboratively.

Contributors can work on independent tasks through GitHub Issues and Pull Requests.

Typical workflow:

```text
GitHub Issue
     ↓
Feature Branch
     ↓
Implementation
     ↓
Pull Request
     ↓
Code Review
     ↓
Merge
```

## Project Status

🚧 **Active Development**

The project is currently in the transition from a detection/tracking prototype toward a complete object analysis system.
