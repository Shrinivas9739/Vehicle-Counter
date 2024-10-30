This project is a Python-based vehicle counting system that uses OpenCV to detect and count vehicles in a video stream. The program processes each frame to identify moving vehicles and counts them as they cross a specified line. This is done through background subtraction, morphological transformations, and contour detection.

Features:

1)Counts vehicles in real-time as they cross a designated counting line.
2)Uses background subtraction to distinguish moving vehicles from the static background.
3)Displays a real-time count of vehicles and shows bounding boxes around detected vehicles.

Prerequisites:

1)Python 3.x
2)OpenCV
3)NumPy

I)Install the required packages by running:

pip install opencv-python numpy

Code Overview:

1)Background Subtraction: Detects moving objects (vehicles) by separating them from the background.
2)Morphological Transformations: Refines the binary mask to improve the shape and connectivity of detected vehicles.
3)Contour Detection: Finds the boundaries of each detected vehicle and counts them when they cross the counting line.
4)Bounding Boxes: Draws a rectangle around each detected vehicle and updates the count in real-time.
