# Eye-Blink-Detection


# Description
Eye blink detection is a computer vision project that tracks a person's eye movements and detects blinks in real-time. This project can be utilized in various applications such as fatigue detection for drivers, controlling devices using eye gestures, or interactive systems for differently-abled individuals.

The project uses Python and OpenCV along with a pre-trained facial landmark detection model. The model identifies key facial points to calculate the Eye Aspect Ratio (EAR), a metric that decreases significantly when an eye blink is detected.

# Features
Real-time eye blink detection using a webcam.
Visual indicators to display the status of the eyes (open or closed).
Captures blink counts and displays them on the screen.

# Prerequisites
Ensure you have the following installed:

Python 3.7 or above
OpenCV
dlib
imutils
numpy
Install dependencies using the command:


pip install opencv-python dlib imutils numpy  

# How It Works
Facial Landmark Detection:

Uses dlib's shape_predictor_68_face_landmarks.dat model to locate 68 facial landmarks.
Specific points around the eyes are used for blink detection.
Eye Aspect Ratio (EAR):

EAR is calculated using the vertical and horizontal distances between eye landmarks.
A significant drop in EAR indicates a blink.
Blink Detection:

Blinks are counted based on EAR thresholds and timing conditions.

# Usage
Clone the repository or download the script.
Download the pre-trained model shape_predictor_68_face_landmarks.dat from dlib's website.
Extract and place the model in the project directory.
Run the script:

python eye_blink_detection.py  
Use a webcam to start real-time eye blink detection.

# Applications
Driver drowsiness detection.
Interactive games or applications.
Health monitoring systems.

# Future Enhancements
Integrate with fatigue detection systems for long-duration tasks.
Extend functionality to detect winks and other eye gestures.
Add support for multi-camera setups.

# Acknowledgments
This project leverages the power of OpenCV, dlib, and Python to perform efficient real-time blink detection. Thanks to the open-source community for their resources and tools.
