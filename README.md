
# Text Detection and Extraction using OpenCV and OCR

This project demonstrates how to use **OpenCV** and **Tesseract-OCR** to detect and extract text from images. The workflow involves:

1. **Image Processing**: OpenCV is used to process the image (grayscale conversion, thresholding, and contour detection).
2. **Text Recognition**: Tesseract-OCR is employed to recognize and extract text from the processed image.
3. **Output**: The extracted text is saved to a file for further use.

## About

This tool is designed for applications such as digitizing printed documents and efficiently extracting information from images. It identifies text regions, extracts the text, and saves the results in a `.txt` file.

## Prerequisites

### Required Installations

- **OpenCV**: For image processing tasks.
- **Pytesseract**: A Python wrapper for Tesseract-OCR.
- **Tesseract-OCR Executable**: Install Tesseract-OCR from [GitHub](https://github.com/tesseract-ocr/tesseract).

### Installation Commands

Install the Python packages:

```bash
pip install opencv-python pytesseract
```

Download and install Tesseract-OCR, and note the installation path (e.g., `C:\Program Files\Tesseract-OCR\tesseract.exe`).

## Steps to Run the Program

1. **Install Required Packages**:

   ```bash
   pip install opencv-python pytesseract
   ```

2. **Download and Install Tesseract-OCR**:

   Download Tesseract-OCR from [here](https://github.com/tesseract-ocr/tesseract) and install it. Note the installation path.

3. **Update the Tesseract Path in the Script**:

   Open the script and update the Tesseract-OCR path as follows:

   ```python
   pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
   ```

4. **Run the Program**:

   Execute the script:

   ```bash
   python text_detection_extraction.py
   ```

5. **Enter the Image Path**:

   When prompted, enter the path to the image you want to process (ensure the path is correct).

6. **View the Output**:

   The recognized text will be saved in a file named `recognized.txt` in the same directory as the script.

## Project Structure

```
text-detection-extraction/
│
├── text_detection_extraction.py  # Main script for text detection and extraction
├── recognized.txt                # Output file for extracted text
└── README.md                     # Project documentation
```

## Applications

- Digitizing printed documents for archiving or editing.
- Extracting data from receipts, forms, or images.
- Automating data entry tasks.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [OpenCV](https://opencv.org/): Open-source computer vision library.
- [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract): OCR engine for text recognition.

---


