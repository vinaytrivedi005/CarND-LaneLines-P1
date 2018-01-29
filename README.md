# **Finding Lane Lines on the Road** 

Overview
---

This project contains a simple code pipeline to identify lanelines from a video footage.

Requirements
---

This project needs `Python 3.5` and `Open CV` library.

Pipeline
---

1. Convert image into gray scale by using `grayscale()` function.
2. Apply gaussian blur on gray scalled image using `gaussian_blur()` function.
3. Apply canny edge detection using `canny()` function to detect edges.
4. Define region of interest in image using `region_of_interest()` function as lanelines are always in lower part of image when image is taken from driver seat.
5. Apply hough line transform using `hough_lines()` to identify and draw lanelines in image.
6. Apply detected lanelines in red to original image to show as lanelines.

Short comings
---

This project can only identify lanelines in straight road. It do not work well if lanelines have curves and video footage has light differences in it.

Improvements
---

Improvements can be made to identify lanelines in different light conditions and lanelines with curves.