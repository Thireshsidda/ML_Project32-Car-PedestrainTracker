# ML_Project32-Car-PedestrainTracker

### Car and Pedestrian Tracker with OpenCV
This project implements a real-time car and pedestrian detection system using OpenCV and pre-trained Haar Cascades.

### Functionality
Detects cars and pedestrians in images and videos.

Draws bounding boxes around detected objects.

### Requirements
Python 3.x

OpenCV library (pip install opencv-python)

### Usage
##### Download pre-trained Haar Cascades:
You can find these online. The sample file paths provided (cars.xml and haarcascade_fullbody.xml) might need to be replaced with the actual locations of your downloaded files.

##### Save the code:
Save the provided code as a Python file (e.g., car_pedestrian_tracker.py).

##### Run the script (image processing):
Update the img_file path to point to your desired image.

Run the script from your terminal: python car_pedestrian_tracker.py

##### Run the script (video processing):
Update the video_file path to point to your video file.

Run the script from your terminal: python car_pedestrian_tracker.py

#### Note: 
The script will display the image/video with bounding boxes around detected cars and pedestrians. Press 'q' to quit the program.

### Haar Cascade Files (XML)
The provided samples (cars.xml and haarcascade_fullbody.xml) are examples of Haar Cascade classifier files. These files contain pre-trained information for detecting specific objects (cars and pedestrians in this case). You can find various Haar Cascade files online for different object categories.

### Explanation:

The script first loads the image/video and the pre-trained Haar Cascade classifiers for cars and pedestrians.

It then converts the image/video frames to grayscale (required for Haar Cascade processing).

The detectMultiScale function from OpenCV is used to identify car and pedestrian regions in the grayscale frame.

For each detected object, a bounding box is drawn on the original frame.

Finally, the script displays the processed image/video with bounding boxes.

### Enhancements
Explore other Haar Cascade classifiers for different object types.

Implement object tracking algorithms to follow detected objects across frames.

Improve accuracy by experimenting with different Haar Cascades or training your own.

Add functionalities like object counting or classification probabilities.
