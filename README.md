# License Plate Recognition System

A computer vision and OCR-based License Plate Recognition (LPR) system developed using Python, OpenCV, and EasyOCR.

The project processes vehicle images to identify the license plate region and extract the plate text using image processing and optical character recognition techniques.

## Overview

License Plate Recognition combines image processing and OCR to automatically identify and read license plates from vehicle images.

This project implements an LPR pipeline that:

1. Reads the input vehicle image
2. Converts the image to grayscale
3. Applies image smoothing and noise reduction
4. Performs edge detection
5. Detects contours to identify potential license plate regions
6. Applies a mask to isolate the detected region
7. Crops the license plate area
8. Uses EasyOCR to extract the license plate text
9. Renders the recognition result

## Technologies Used

- Python
- OpenCV
- EasyOCR
- NumPy
- Matplotlib
- imutils

## Processing Pipeline

```text
Input Vehicle Image
        ↓
Image Preprocessing
        ↓
Grayscale Conversion
        ↓
Noise Reduction
        ↓
Canny Edge Detection
        ↓
Contour Detection
        ↓
License Plate Region Detection
        ↓
Masking & Cropping
        ↓
EasyOCR
        ↓
License Plate Text
