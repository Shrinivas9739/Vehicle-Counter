This project is a Python-based vehicle counting system that uses OpenCV to detect and count vehicles in a video stream. The program processes each frame to identify moving vehicles and counts them as they cross a specified line. This is done through background subtraction, morphological transformations, and contour detection.

**Features**:

1)Counts vehicles in real-time as they cross a designated counting line.
2)Uses background subtraction to distinguish moving vehicles from the static background.
3)Displays a real-time count of vehicles and shows bounding boxes around detected vehicles.

**Prerequisites:**

1)Python 3.x

2)OpenCV

3)NumPy

**Install the required packages by running:**

pip install opencv-python numpy

**Code Overview:**

1)Background Subtraction: Detects moving objects (vehicles) by separating them from the background.

2)Morphological Transformations: Refines the binary mask to improve the shape and connectivity of detected vehicles.

3)Contour Detection: Finds the boundaries of each detected vehicle and counts them when they cross the counting line.

4)Bounding Boxes: Draws a rectangle around each detected vehicle and updates the count in real-time.

**Code Explanation:**

I)Initialization: Opens the video, sets parameters for counting, and initializes the background subtractor.

II)Processing Frames: For each frame, the code applies:

II.1)Grayscale and Blur: Simplifies each frame by converting it to grayscale and reducing noise with a Gaussian blur.

II.2)Background Subtraction: Detects moving objects and produces a binary mask.

II.3)Dilation and Morphological Closing: Refines detected objects by connecting parts and removing noise.

II.4)Contour Detection: Finds each vehicle’s contour and draws bounding boxes around valid vehicles.

II.5)Counting: Updates the vehicle count whenever a vehicle crosses the counting line.

**The program displays:**

1)Real-time video with detected vehicles and a bounding box for each vehicle.

2)A counting line where vehicles are detected as they cross.

3)The total vehicle count in real time.

**Note**: To get the video used in this project, download it from the file provided in this repository.
