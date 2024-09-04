# Face-Grouping-Using-Computer-Vision
This project is a facial recognition-based photo organizer that efficiently sorts and categorizes images based on detected faces. It uses a deep neural network (DNN) with the Caffe model for face detection and employs the face_recognition library for face encoding and matching.

## Project Structure
  * ***model_dnn.py***: The main script that handles the entire process of face detection, encoding, and photo organization.
  * ***deploy.prototxt***: The Caffe model architecture file. This defines the structure of the neural network used for face detection.
  * ***res10_300x300_ssd_iter_140000.caffemodel***: The Caffe model weights file. This contains the pre-trained weights for the neural network.

## Ensure you have the following files in the project directory:

  * model_dnn.py
  * deploy.prototxt
  * res10_300x300_ssd_iter_140000.caffemodel

## Usage
  * Prepare Known Faces:
    Place images of known individuals in a directory (e.g., Faces).
    Run the Script:
    Specify the paths for the known faces directory, event photos directory, and the output directory within model_dnn.py.

## Execute the script:
  * python model_dnn.py

## Organized Output:
  * The script will create a new directory (output_using_DNN by default) and sort photos into subdirectories named after the recognized individuals.

## Example Directories Structure
```
project-root/
│
├── model_dnn.py
├── deploy.prototxt
├── res10_300x300_ssd_iter_140000.caffemodel
├── Faces/
│   ├── person1.jpg
│   ├── person2.jpg
│   └── ...
├── Testing Faces/
│   ├── event_photo1.jpg
│   ├── event_photo2.jpg
│   └── ...
└── output_using_DNN/
    ├── person1/
    │   ├── event_photo1.jpg
    │   └── ...
    ├── person2/
    │   ├── event_photo2.jpg
    │   └── ...
    └── ...
```
