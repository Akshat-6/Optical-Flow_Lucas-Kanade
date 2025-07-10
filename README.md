

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


 

