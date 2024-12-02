---
title: "Depth Based Multi-Human Skeletal Pose Detection."
excerpt: "An AI-algorithm based motion detector that utilizes a depth camera for accurate motion capture.<br/><img src='/images/500x300.png'>"
collection: portfolio
youtubeId: _Jam5S9RhWI
---

{% include youtubePlayer.html id=page.youtubeId %}
<br>
## Project Use Case 
Most AI-based humanoid motion trackers rely on 2D image trackers which excludes depth accuracy as they work in pixel spaced. This project aimed to bridge that gap by utilizing AI RGB image pose detection and mapping those coordinates to a depth map for processing in real world metered coordinates.

## Project Functionality
The used depth camera was the intel d435 depth camera where the SDK was downloaded as a git submodule, compiled and built with CMake, and the built shared libraries acting as Python C++ wrappers are integrated into the Python virtual environment.  The OpenCV, YOLOv8 and Google MediaPipe libraries are set up with PIP. First the realsense SDK begins streaming both RGB and depth video feeds into the main Python pipeline, where the depth frames are aligned to the RGB feed for accurate coordinate mapping. 

Next a YOLO Tracker is run over the RGB stream where only people are detected and sub-numpy matrices are extracted from where the bounding boxes are normally gathered. The matrices are padded so that MediaPipe’s pose detection will more accurately apply the skeletal model. DIfferent people will receive a UUID per their appearance and detection within YOLO.

MediaPipe’s pose detection only works for one human at a time, so it was necessary to extract multiple human bounding boxes for multi-person support. The reason for MediaPipe being selected as the skeletal tracker, was due to its use of state space physics in its AI pose detection and inbuilt coordinate filters. Once a sub-matrix is fed into the MediaPipe function, the human joint locations are recorded and the wrists and nose points are drawn in opencv over the aligned depth image.

For demonstration sake, the OpenCV drawn joint circles will scale in relation to where the depth coordinates (gathered from the aligned depth frame) depth value. This showcases that a robot utilizing this framework will be able to accurately assess how far a human’s pose is in relationship to itself. 

## Next Steps
Going forward this project will be built and configured for GPU usage for faster AI algorithm deployments.
MediaPipe’s application in this project was written in a way to generate a detection thread and will thus be optimized to use multiple cores for different image extractions scaled by the number of detected bounding boxes.
Multi object support will be written into the YOLOv8 component so it can also detect if the person is holding objects.

