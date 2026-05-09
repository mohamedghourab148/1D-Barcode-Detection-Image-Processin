
# 1D Barcode Detection using Image Processing

This project implements an orientation-independent 1D barcode detection system using classical image processing techniques. The goal is to accurately detect and localize one or multiple barcodes in an image without using machine learning.

## Features
- Detects barcodes with varying sizes and orientations
- Robust to noise and cluttered backgrounds
- Handles merged and stacked barcodes
- Removes duplicate detections using Non-Maximum Suppression (NMS)

## Techniques Used
- Grayscale conversion & Gaussian blurring
- Sobel gradient edge detection
- Otsu thresholding
- Morphological operations (opening & closing)
- Contour analysis & rotated bounding boxes
- Projection-based and watershed-based splitting
- Non-Maximum Suppression using IoU and centroid distance

## Technologies
- Python
- OpenCV
- NumPy
- Matplotlib
- Jupyter Notebook / Google Colab

## Sample Result
Input images may contain multiple, rotated, or overlapping barcodes.  
The system outputs bounding boxes around each detected barcode.

## Future Work
- Integrate barcode decoding (EAN-13, UPC, Code128)
- Handle blurred or partially occluded barcodes
- Extend to real-time video barcode detection
