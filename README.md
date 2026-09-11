# License Plate Recognition System

A computer vision and Optical Character Recognition (OCR) based License Plate Recognition (LPR) system developed using Python, OpenCV, and EasyOCR.

## Overview

This project processes vehicle images to identify a potential license plate region and extract the text from the detected region using image processing and OCR techniques.

The implementation follows a sequence of image preprocessing, edge detection, contour detection, region extraction, and OCR-based text recognition.

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
Grayscale Conversion
        ↓
Image Smoothing / Noise Reduction
        ↓
Canny Edge Detection
        ↓
Contour Detection
        ↓
Potential License Plate Region
        ↓
Masking & Region Extraction
        ↓
License Plate Crop
        ↓
EasyOCR
        ↓
Extracted License Plate Text
```

## How It Works

### 1. Image Preprocessing

The input vehicle image is loaded and converted to grayscale. Image smoothing is applied to reduce noise and improve the results of subsequent image-processing operations.

### 2. Edge Detection

Canny edge detection is used to identify important edges in the processed image.

### 3. Contour Detection

Contours are detected from the edge image and evaluated to identify regions that may correspond to a license plate.

### 4. License Plate Region Extraction

A mask is created around the selected region and used to isolate and crop the potential license plate area from the original image.

### 5. OCR-Based Text Recognition

EasyOCR is applied to the extracted license plate region to detect and recognize the characters present in the image.

## Key Concepts Demonstrated

- Image preprocessing
- Grayscale conversion
- Image smoothing
- Canny edge detection
- Contour detection
- Image masking and cropping
- Region extraction
- Optical Character Recognition (OCR)
- Python-based computer vision
- Processing of real-world image data

## Project Structure

```text
LPR_Sytems/
│
├── LPR_Sytem_SourceCode.ipynb
├── LPR_System_Report.pdf
└── README.md
```

### Files

**`LPR_System_SourceCode.ipynb`**  
Jupyter Notebook containing the implementation of the image-processing and OCR pipeline.

**`LPR_System_Report.pdf`**  
Project report containing additional information about the License Plate Recognition System.

## Requirements

Install the Python libraries used by the project:

```bash
pip install opencv-python numpy matplotlib imutils easyocr
```

## Running the Project

1. Clone the repository:

```bash
git clone https://github.com/kr492/LPR_Sytems.git
```

2. Open the project directory.

3. Launch `LPR_Sytem_SourceCode.ipynb` using Jupyter Notebook or JupyterLab.

4. Install the required dependencies if they are not already available.

5. Run the notebook cells in sequence and provide the required input image when prompted by the implementation.

## Results

The system uses image-processing techniques to locate a potential license plate region and EasyOCR to extract text from the selected region.

The complete implementation and project report are available in this repository.

## Future Improvements

- Improve license plate detection under different lighting and image conditions.
- Extend the system to process video streams and multiple vehicles.
- Improve OCR results through additional image preprocessing.
- Add support for different license plate formats.
- Develop a real-time application or deployment interface.

## Project Report

The detailed project report is available in:

`LPR_System_Report.pdf`

## Author

**Mohammad Kaif Raza Ansari**

- GitHub: https://github.com/kr492
- LinkedIn: https://www.linkedin.com/in/kaif-data-engineer/
