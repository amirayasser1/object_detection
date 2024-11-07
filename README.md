# object_detection
## Model Selection and Setup:

I used the YOLOv8 pre-trained model, known for its high accuracy and speed in object detection tasks.
The model was loaded using the Ultralytics library, which simplifies model handling and inference.
Video Input and Processing:

The system reads frames from a video file using OpenCV's VideoCapture.
To optimize processing, I resized frames to a consistent resolution, balancing detection speed and accuracy.
Detection and Visualization:

For each frame, I used YOLOv8’s .predict() function to detect objects. The model outputs bounding boxes, class IDs, and confidence scores.
Bounding boxes and labels were drawn on each detected object using OpenCV’s rectangle() and putText() functions. Labels included the class name .

## User Interaction and Display:

I set up OpenCV’s imshow() to display frames with detected objects in real time.
The program allows users to stop the detection by pressing the Esc key.
