# Live Car Detection with OpenCV

This project demonstrates a simple car detection system using OpenCV's Haar Cascade Classifier. The script captures video from a webcam in real-time, detects cars in each frame, and displays the video feed with bounding boxes drawn around detected cars.

## Features

- Real-time car detection using a pre-trained Haar Cascade Classifier.
- Bounding boxes are drawn around detected cars in the video feed.
- Live video feed displayed in a window with detection results.
- Press the 'q' key to exit the application.

## Prerequisites

- Python 3.x
- OpenCV library

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/ANBAZHAGAN-007
    cd repositoryname
    ```

2. **Install the required Python package:**

    ```bash
    pip install opencv-python
    ```

3. **Download the Haar Cascade XML file:**

    Ensure you have the `cars.xml` file for the Haar Cascade Classifier. You can obtain it from the [OpenCV GitHub repository](https://github.com/opencv/opencv/tree/master/data/haarcascades).

4. **Place the `cars.xml` file in the `Live_Car_Detector` directory** or modify the script to point to the location where you store the XML file.

## Usage

1. **Run the script:**

    ```bash
    python car_detection.py
    ```

2. The video capture window will open, and the script will start detecting cars in real-time.

3. **Press the 'q' key** to exit the application and close the video capture window.

## Code Overview

- **Loading the Haar Cascade Classifier:**
  
  The `cv2.CascadeClassifier('Live_Car_Detector/cars.xml')` function loads the pre-trained classifier for car detection.

- **Initializing Video Capture:**

  `cv2.VideoCapture(0)` initializes the video capture from the default webcam.

- **Processing Each Frame:**

  The script reads each frame from the webcam, converts it to grayscale, and applies the car detection algorithm.

- **Drawing Bounding Boxes:**

  Detected cars are highlighted with red rectangles.

- **Displaying Results:**

  The processed frames are shown in a window named 'Car Detection'.

- **Exiting the Application:**

  The application runs in an infinite loop until the 'q' key is pressed.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This project uses OpenCV for computer vision tasks.
- Haar Cascade Classifier for car detection is provided by OpenCV.
