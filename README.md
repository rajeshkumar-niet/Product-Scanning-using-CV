# Real-Time Expiry Date Detection Using OCR and Webcam

## Overview
This project automates the detection and extraction of expiry and manufacturing dates from product labels using Optical Character Recognition (OCR). The system captures images via a webcam, processes them in real-time using EasyOCR, and extracts date-related information such as expiry and manufacturing dates. The detected data is logged in a CSV file with a timestamp, making it useful for industries such as pharmaceuticals, food, and retail management.

## Features
- **Real-time image capture**: Captures images using the webcam directly within the Python environment.
- **OCR for text extraction**: Uses EasyOCR to detect and extract text from product labels.
- **Date extraction**: Identifies expiry and manufacturing dates using keyword-based matching and regular expressions.
- **CSV logging**: Logs the extracted dates, along with a timestamp, into a CSV file.
- **Data persistence**: Appends data to an existing file in Google Drive or creates a new one.

## Technologies Used
- **Python**: Main programming language for the project.
- **EasyOCR**: Optical Character Recognition library used to extract text from images.
- **OpenCV**: Library for handling image processing and displaying results.
- **Matplotlib**: Used for visualizing the annotated images.
- **Google Colab**: For running the code in the cloud environment with webcam support.
- **CSV**: Used for storing the extracted dates and timestamps.

## Installation and Setup
1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd <project-directory>
   ```

2. **Install the required dependencies**:
   ```bash
   pip install easyocr opencv-python matplotlib
   ```

3. **Run the Python script**:
   - Open the script in a Python environment like Google Colab or Jupyter Notebook.
   - Run the cells in sequence to start capturing images and extracting expiry and manufacturing dates.

4. **Google Drive integration**:
   - The detected data will be saved in a CSV file, and if the file already exists in Google Drive, new data will be appended.

## Usage
1. The system will start by capturing images from the webcam.
2. After each capture, the text will be extracted, and the expiry and manufacturing dates will be identified.
3. The detected dates will be saved in a CSV file for future reference.

## Future Improvements
- Support for additional languages for OCR.
- Improve date format detection to handle more complex date patterns.
- Add email notification feature for expired products.

