A Collection of Computer Vision Scripts using OpenCV

This repository is a curated collection of Python scripts demonstrating various fundamental concepts and techniques in computer vision using the OpenCV library. Each script is a self-contained example designed to be easy to understand, execute, and adapt for your own projects.

Whether you're a beginner learning the basics or an experienced developer looking for a quick reference, these scripts provide practical examples of common computer vision tasks.

Table of Contents

Core Concepts Covered

Scripts Breakdown

Prerequisites

Usage

Core Concepts Covered

This collection spans a wide variety of topics, including:

Video I/O: Reading from video files and capturing from a webcam.

Image Processing: Color space conversions, thresholding, and masking.

Drawing and Annotation: Adding lines, shapes, and text to images.

Object Detection & Recognition: Template matching, feature matching, and corner detection.

Image and Video Analysis: Foreground extraction and background subtraction.

Dataset Creation: Tools for downloading and preparing images for machine learning tasks.

Scripts Breakdown

Here is a detailed description of each script in the repository:

Script Name	Description
pic1.py	Read and Display Video: Opens a video file (hello.wmv), reads it frame-by-frame, converts each frame to grayscale, and displays the result in a window.
pic2.py	Capture and Save Video: Captures video from a webcam, displays the live feed in grayscale, and simultaneously saves the original color footage to a new video file (output.avi).
pic3.py	Drawing on Images: Demonstrates how to draw various shapes (lines, rectangles, circles, polygons) and write text on an image using OpenCV's built-in functions.
pic4.py	Image ROI and Masking (Logo Overlay): A practical example of how to overlay a small logo onto a larger image. It uses Region of Interest (ROI), masking, and bitwise operations to seamlessly blend the images.
pic5.py	Image Thresholding Techniques: Shows several methods for image thresholding, including simple binary thresholding, adaptive Gaussian thresholding, and Otsu's binarization method, which is excellent for images with non-uniform lighting.
pic6.py	Template Matching: A simple object detection technique. It searches for a small template image within a larger source image and draws rectangles around all the locations where a match is found.
pic7.py	Foreground Extraction with GrabCut: Implements the GrabCut algorithm, an interactive method for intelligently separating a foreground object from the background based on an initial rectangular selection.
pic8.py	Harris Corner Detection: An implementation of the Harris Corner Detection algorithm, a fundamental technique for identifying corners and points of interest in an image.
pic9.py	Sub-Pixel Corner Refinement: Extends the Harris detector by refining the detected corner locations to achieve sub-pixel accuracy, which is crucial for high-precision tasks like camera calibration.
pic10.py	Feature Detection and Matching (ORB): Demonstrates how to use the ORB (Oriented FAST and Rotated BRIEF) algorithm to detect keypoints in two different images and find the best matches between them.
pic11.py	Background Subtraction for Video: Analyzes a video of moving objects (people-walking.mp4) and creates a foreground mask to isolate the moving elements (the people) from the static background.
pic12.py	Building an Image Dataset: A utility script for machine learning preparation. It downloads a list of images from ImageNet URLs, resizes them, and creates a bg.txt file, which is used to describe negative images when training object detection classifiers (like Haar Cascades).
Prerequisites

To run these scripts, you will need Python 3 installed, along with the following libraries:

OpenCV: For all core computer vision functions.

NumPy: For numerical operations and array manipulation.

Matplotlib: Used in some scripts for displaying images and plots.

You can install all the required libraries using pip:

code
Bash
download
content_copy
expand_less
pip install opencv-python numpy matplotlib
Usage

Clone the repository:

code
Bash
download
content_copy
expand_less
git clone https://github.com/your-username/opencv-computer-vision.git
cd opencv-computer-vision

Provide Input Files:
Most scripts require specific image or video files to run. Make sure you have the necessary files in the same directory as the script, or update the file paths within the scripts.

Required files include: hello.wmv, pic1.jpg, 3D-Matplotlib.png, mainlogo.png, bookpage.jpg, opencv-template-matching-python-tutorial.jpg, opencv-template-for-matching.jpg, opencv-corner-detection-sample.jpg, opencv-feature-matching-template.jpg, opencv-feature-matching-image.jpg, people-walking.mp4.

Run a script from your terminal:
Navigate to the repository's directory and run any script using Python.

code
Bash
download
content_copy
expand_less
# Example:
python pic6.py

Press the 'q' key or the ESC key (depending on the script) to close the display window and terminate the script.
