# Real-Time Object Detection with YOLOv8

This project demonstrates real-time object detection using the YOLOv8 (You Only Look Once) model, implemented with the help of OpenCV and PyTorch. The application captures live video from the webcam and identifies objects in the frame using the pre-trained YOLOv8 model.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Model Details](#model-details)
- [Object Classes](#object-classes)
- [Contributing](#contributing)
- [License](#license)

## Installation

To run this project, you'll need Python and several dependencies. You can install the required packages using the following commands:

```bash
pip install ultralytics
pip install opencv-python
pip install torch
````
Ensure you have a compatible GPU and CUDA installed for optimal performance. If CUDA is not available, the model will default to CPU.

##Usage
To start the object detection application, simply run the script:

```bash
python object_detection.py
```
The script will open a window displaying the webcam feed. The model will detect objects in real-time and draw bounding boxes around them, displaying the class names and confidence scores.
Key Components
Webcam Feed: Captures live video using OpenCV.
YOLOv8 Model: Loads a pre-trained model for object detection.
Bounding Boxes: Draws boxes around detected objects and labels them with class names.
Press q to exit the application.

Model Details
The application uses the YOLOv8 model, known for its high accuracy and speed in object detection tasks. YOLO (You Only Look Once) is a state-of-the-art, real-time object detection system that predicts bounding boxes and class probabilities directly from full images.

The model is loaded from a pre-trained weight file yolov8n.pt, which is a lightweight version suitable for real-time applications. The model is implemented using the ultralytics library, and it leverages the power of PyTorch for deep learning tasks.

Object Classes
The YOLOv8 model can detect a wide range of objects, as defined in the COCO dataset. Here are some of the classes the model can recognize:

Person
Bicycle
Car
Motorbike
Aeroplane
Bus
Train
Truck
Boat
Traffic light
Fire hydrant
Stop sign
Parking meter
Bench
Bird
Cat
Dog
Horse
Sheep
Cow
Elephant
Bear
Zebra
Giraffe
Backpack
Umbrella
Handbag
Tie
Suitcase
Frisbee
Skis
Snowboard
Sports ball
Kite
Baseball bat
Baseball glove
Skateboard
Surfboard
Tennis racket
Bottle
Wine glass
Cup
Fork
Knife
Spoon
Bowl
Banana
Apple
Sandwich
Orange
Broccoli
Carrot
Hot dog
Pizza
Donut
Cake
Chair
Sofa
Potted plant
Bed
Dining table
Toilet
TV monitor
Laptop
Mouse
Remote
Keyboard
Cell phone
Microwave
Oven
Toaster
Sink
Refrigerator
Book
Clock
Vase
Scissors
Teddy bear
Hair drier
Toothbrush
The full list of object classes is available in the script's classNames array.

Contributing
Contributions to this project are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.

To contribute:

Fork the Repository: Click the "Fork" button at the top right of this page.

Clone the Repository: Clone your fork to your local machine using the following command:

```bash
git clone https://github.com/your-username/Real-Time-Object-Detection-Model.git

```

