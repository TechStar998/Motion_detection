# Motion_detection
# AI Fitness Motion Detector

A computer vision-based fitness tracking application that uses MediaPipe Pose Estimation and OpenCV to detect human body landmarks in real time and count exercise repetitions automatically.

The system tracks joint movements, calculates elbow angles, and identifies complete bicep curl repetitions through webcam input.

##  Tech Stack

* Python
* OpenCV
* MediaPipe
* NumPy

##  How It Works

1. Captures video frames from webcam.
2. Detects body landmarks using MediaPipe Pose.
3. Extracts shoulder, elbow, and wrist coordinates.
4. Calculates elbow angle using vector mathematics.
5. Detects arm movement stages:

   * Down Position → Angle > 160°
   * Up Position → Angle < 30°
6. Increments repetition counter after a complete curl.

##  System Workflow

Webcam Input → Pose Detection → Landmark Extraction → Angle Calculation → Stage Detection → Rep Counter Update


