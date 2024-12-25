
Lane Detection System
=====================

A Python-based project that detects lanes in a video using computer vision techniques. This system leverages the Canny edge detection algorithm, Region of Interest (ROI) masking, and the Hough Line Transform to identify lane lines.

Features
--------

*   Detects lane lines from a given video feed.
*   Overlays detected lanes on the original video for visualization.
*   Customizable parameters for edge detection and line detection.

Requirements
------------

Ensure the following libraries are installed:

*   **Python 3.x**
*   **OpenCV** (`cv2`)
*   **NumPy** (`numpy`)
*   **Matplotlib** (`matplotlib`) \[Optional for debugging\]

Install the required libraries using:

    pip install opencv-python numpy matplotlib

How It Works
------------

### 1\. Read the Video

The video is read frame by frame using OpenCV's `cv2.VideoCapture()`.

### 2\. Convert Frame to Grayscale

Each frame is converted to grayscale for simplicity and efficiency.

### 3\. Apply Edge Detection

The Canny edge detection algorithm is used to detect edges in the frame.

### 4\. Define Region of Interest (ROI)

A trapezoidal region of interest is applied to focus on the road area, excluding irrelevant parts.

### 5\. Apply Hough Transform

The Hough Line Transform is used to detect straight lines (lane lines).

### 6\. Overlay Detected Lines

The detected lane lines are drawn over the original frame for visualization.


Output
------

The system displays the video with detected lanes highlighted in real-time.

Customization
-------------

*   Adjust Canny edge detection thresholds for better edge detection.
*   Modify ROI coordinates to suit different road layouts.
*   Tweak Hough Transform parameters to detect lanes more accurately.

License
-------

This project is open-source and available under the MIT License.
