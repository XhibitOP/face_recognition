#face Recognition Application

This project is a Python-based face recognition application that allows users to capture, compare, and store photos using a graphical user interface (GUI). It uses a webcam to capture images, detects faces, and compares them for similarities. The project also logs photo records in an SQLite database.

Features

Capture Reference Photo: Take a reference photo to compare against.

Capture and Compare: Capture a new photo and compare it with the reference.

Face Detection: Detect faces using OpenCV's Haar cascades.

Similarity Check: Compare faces using the Structural Similarity Index (SSIM).

Photo Logging: Log photo details, timestamps, and match results in an SQLite database.

GUI: User-friendly interface built with Tkinter.

Prerequisites

Before running the application, ensure you have the following:

Python 3.7 or higher

Required Python libraries:

OpenCV

Tkinter (comes pre-installed with Python)

PIL (Pillow)

SQLite3 (comes pre-installed with Python)

Scikit-image

Installation

Clone or download this repository.

Install the required Python libraries:

pip install opencv-python-headless scikit-image pillow

Run the script:

python <script_name>.py

Directory Structure

|-- face_recognition_app/
    |-- static/
        |-- images/   # Directory to store captured photos
    |-- PHOTOS.db      # SQLite database file
    |-- script.py      # Main application script
    |-- README.md      # Project documentation

Usage

Launch the application:
Run the script.py file in your terminal or IDE.

Capture Reference Photo:

Click the "Capture Reference Photo" button.

A reference photo will be captured and displayed in the left panel.

Capture New Photo:

Click the "Capture New Photo" button.

A new photo will be captured and displayed in the right panel.

Compare Photos:

The application will compare the new photo with the reference photo.

Results will be displayed (Matched or Not Matched).

View Logs:

All photo records are saved in the PHOTOS.db database.

Notes

Ensure your webcam is functional.

Images are stored in the static/images directory.

Detected faces are compared based on similarity scores.

Future Enhancements

Implement additional face recognition techniques (e.g., deep learning).

Add an option to export logs.

Enhance the GUI for better user experience.

License

This project is licensed under the MIT License.


