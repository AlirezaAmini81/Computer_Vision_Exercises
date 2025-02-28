# Computer Vision Exercises

This repository contains the implementation of various computer vision algorithms as part of a research project. The exercises include edge detection, color segmentation, texture-based segmentation, histogram of oriented gradients (HOG), and the SIFT algorithm for scene stitching.

## Table of Contents

1. [Edge Detection](#edge-detection)
   - [Prewitt](#prewitt)
   - [Kirsch](#kirsch)
   - [Marr-Hildreth](#marr-hildreth)
   - [Canny](#canny)
2. [Color Segmentation](#color-segmentation)
3. [Texture-based Segmentation](#texture-based-segmentation)
4. [Histogram of Oriented Gradients (HOG)](#histogram-of-oriented-gradients-hog)
5. [SIFT Algorithm for Scene Stitching](#sift-algorithm-for-scene-stitching)

## Edge Detection

### Prewitt
The Prewitt edge detection algorithm uses convolution masks to compute gradients in both horizontal and vertical directions, calculating the magnitude of the gradients to identify edges.

### Kirsch
The Kirsch edge detection algorithm uses eight convolution masks oriented at 45-degree intervals to capture gradients in different directions and identify edges.

### Marr-Hildreth
The Marr-Hildreth algorithm applies a Gaussian filter followed by the Laplacian and zero-crossing operation to detect edges.

### Canny
The Canny edge detection algorithm uses a multi-stage process involving Gaussian filtering, gradient calculation, non-maximum suppression, and double thresholding to detect edges.

## Color Segmentation
Color segmentation is performed by converting the image to HSV color space and using k-means clustering to segment the image into different regions.

## Texture-based Segmentation
Texture-based segmentation involves creating a bank of Gabor filters and convolving them with the original image, followed by k-means clustering based on the detected textures.

## Histogram of Oriented Gradients (HOG)
The HOG algorithm computes image descriptors by dividing the image into small cells, computing gradients, and quantizing them into orientation bins.

## SIFT Algorithm for Scene Stitching
The SIFT algorithm is used for scene stitching by detecting keypoints, computing descriptors, matching descriptors between images, estimating perspective transformation, and blending the images to create a panorama.

## Results
### Edge Detection
The results of the edge detection algorithms on various images demonstrate the differences in their edge detection capabilities.

![Edge Detection Results](images/edge_detection_results.png)

### Color Segmentation
The color segmentation results for different k values show how increasing the number of clusters affects the segmentation.

![Color Segmentation Results](images/color_segmentation_results.png)

### Texture-based Segmentation
The texture-based segmentation results show how varying parameters of Gabor filters affect the segmentation.

![Texture-based Segmentation Results](images/texture_segmentation_results.png)

### Histogram of Oriented Gradients (HOG)
The HOG results demonstrate the effect of varying parameters such as the number of orientation bins, pixels per cell, and cells per block on the detail and accuracy of the image descriptors.

![HOG Results](images/hog_results.png)

### SIFT Algorithm for Scene Stitching
The SIFT results show the effect of varying parameters such as sigma and contrast threshold on the quality of the image stitching.

![Scene Stitching Results](images/scene_stitching_results.png)

---

### Prerequisites

Ensure you have the following libraries installed:

- OpenCV
- NumPy
- Scikit-Image

