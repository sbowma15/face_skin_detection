face_skin_detection.py

This Python script, face_skin_detection.py, is designed for detecting faces in images using Haar cascades and subsequently applying a skin detection algorithm based on RGB thresholds. The script utilizes the OpenCV library for image processing and Matplotlib for visualization.

Prerequisites

Ensure you have the required libraries installed before running the script:

bash
Copy code
pip install opencv-python matplotlib
Usage
Open the script in your Python environment.

Adjust the file paths in the cv.imread function to the location of your input images:

python
Copy code
image1 = cv.imread("/path/to/your/pp1.png")
image2 = cv.imread("/path/to/your/pp2.png")
Run the script.

Output
The script provides the following outputs:

Displays the original images (pp1.png and pp2.png) with rectangles drawn around detected faces.
Saves face cuts as cut1.png and cut2.png.
Displays skin regions detected in the face cuts.
Displays the merged result, where skin regions are overlaid onto the original face cuts.
Displays the final result after applying a median blur to the merged image.
Feel free to experiment with different images and adjust the RGB threshold values in the skin_rgb_threshold function for customized skin detection results.

Notes
The Haar cascade file (haarcascade_frontalface_default.xml) should be located in the specified path ('/content/sample_data/'). Ensure its availability for face detection.

This script serves as a demonstration of face detection and skin detection in images and can be extended or modified for various applications.






