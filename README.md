# Text Detection and Extraction using OpenCV and OCR

This project demonstrates how to use OpenCV and Tesseract-OCR to detect and extract text from images. OpenCV is utilized for image processing tasks such as converting the image to grayscale, applying thresholding, and finding contours. Tesseract-OCR is then employed to recognize and extract text from the processed image. The extracted text is saved to a file for further use.

## About

This project uses OpenCV and Tesseract-OCR to detect and extract text from images. It processes images to identify text regions, extracts the text, and saves it to a file. This tool is useful for digitizing printed documents and extracting information from images efficiently.

## Required Installations

Before running the program, you need to install the following packages:

```sh
pip install opencv-python
pip install pytesseract
```
You need to download and install the Tesseract-OCR executable. You can download it from this link-https://github.com/tesseract-ocr/tesseract

## Steps to Run the Program

### 1.Install Required Packages:
```sh
pip install opencv-python pytesseract
```

### 2.Download and Install Tesseract-OCR:

Download Tesseract-OCR from this link and install it. Note the installation path (e.g., C:\Program Files\Tesseract-OCR\tesseract.exe).

### 3.Update the Tesseract Path in the Script:

Open the script and update the Tesseract-OCR path:
```python
pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
```

### 4.Run the Program:

Execute the script:
```sh
python text_detection_extraction.py
```

### 5.Enter the Image Path:

When prompted, enter the path to the image you want to process. Ensure the path is correct and properly formatted.

### 6.View the Output:

The recognized text will be saved in the recognized.txt file in the same directory.
