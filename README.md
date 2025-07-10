

# Optical-Flow_Lucas-Kanade
Implementation of Lucas–Kanade optical flow to detect and track motion between video frames using OpenCV.

🎥 Optical Flow Detection using Lucas–Kanade Method


This project demonstrates how to detect motion between consecutive video frames using the Lucas–Kanade Optical Flow algorithm, implemented in Python using OpenCV.


🧠 What is Optical Flow?

Optical Flow refers to the pattern of apparent motion of objects, surfaces, and edges in a visual scene caused by relative motion between an observer and the scene.

It is used in:

Motion detection

Object tracking

Video stabilization


📌 Lucas–Kanade Method – Theory

The Lucas–Kanade method is a differential method for optical flow estimation:

Assumes small and consistent motion in a neighborhood

Solves the optical flow equation using least squares in a window around each pixel

Tracks sparse features (corners, high-texture points)


Optical Flow Equation:


I 
x
​
 ⋅V 
x
​
 +I 
y
​
 ⋅V 
y
​
 +I 
t
​
 =0


 Where:

I 
x
​
 ,I 
y
​
 : Spatial image gradients


 I 
t
​
 : Temporal intensity gradient


𝑉
𝑥
,
𝑉
𝑦
V 
x
​
 ,V 
y
​
 : Flow vector to be estimated
 
 
 🎯 Objective



To track motion between frames by calculating pixel-wise displacement vectors.


Visualize motion vectors for selected key points using arrows or trails.


 
📂 Features

Reads two consecutive frames or a video stream

Detects good features to track using cv2.goodFeaturesToTrack()

Applies cv2.calcOpticalFlowPyrLK() for Lucas–Kanade optical flow

Draws motion vectors using lines and circles



📁 Project Structure


optical-flow-lucas-kanade/
├── lucas_kanade_optical_flow.py        # Main script
├── sample_video.mp4                    # Optional video file
├── output_frames/                      # Optional: stored output
├── README.md
└── requirements.txt


🛠️ Technologies Used


Python

OpenCV

NumPy

Matplotlib (for visualization, optional)

🚀 How to Run

Clone the repository:


git clone https://github.com/yourusername/optical-flow-lucas-kanade.git
cd optical-flow-lucas-kanade

Install dependencies:


pip install opencv-python numpy

Run the script:

python lucas_kanade_optical_flow.py

