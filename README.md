# 👓 Motion Tracker with OpenCV

This project highlights my first time learning/working with OpenCV and classical computer vision concepts. More specifically, this project 
tracks the user's movement through their webcam, by implementing the general CV pipeline for motion detection (image preprocessing -> binary motion mask -> bounding box contouring -> centroid tracking).

## 🧰 Tool's
 - Personal webcam

## 💻 Languages/Frameworks:
 - Python (OpenCV)

## 💡 Features
 - Image preprocessing with grayscale + Gaussian blur
 - Binary motion mask created by applying frame differencing and pixel thresholding
 - Cleans regions of motion through morphology (Opening -> Closing) to apply filtered contouring (motion detection)
 - Applies bounding box's to clearly localize/visualize motion regions
 - Computes centroids (centre of motion regions) and stores the previous centroid to enable motion tracking
 - Displays bounding box's, centroids, and tracking lines on live camera feed to show how motion is perceived in real-time
 - Added overlay to indicate when program is actively tracking vs when it is idle

## ❔How to Run:
1. Clone the repository:
```bash
git clone https://github.com/habelk123/Motion-Tracker-Project.git
```
2. Install dependencies:
```bash
pip install opencv-python numpy
```
3. Run the project file:
```bash
motion_tracker_project.py
```
