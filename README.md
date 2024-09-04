# FaceRecognition

FaceRecognition is a Machine Learning project designed to recognize individuals from images, similar to facial recognition technologies used by platforms like Facebook. By leveraging dlib's advanced deep learning models, this project provides a robust solution for face recognition tasks. The system achieves an impressive 99.38% accuracy on the Labeled Faces in the Wild (LFW) benchmark, making it a powerful tool for various applications.

## Features

- **High Accuracy:** 99.38% on the LFW benchmark.
- **Face Recognition:** Identify and verify individuals from images.
- **Real-Time Detection:** Capable of processing webcam input for real-time face recognition.

## Dependencies

To run this project, you need the following:

- **Python 3.x**
- **Numpy**
- **Scipy**
- **Scikit-learn**
- **dlib**

### Optional Extras

- **OpenCV:** Required only for `webcam.py` to capture frames from a webcam.
- **OpenFace:** Required for `./demo-python-files/projecting_faces.py`.

## Procedure

### 1. Clone the Repository

Clone the repository to your local machine and navigate to the project directory.

### 2. Prepare Training Data

- **Create Training Image Folders**

  Create a directory named `training-images`. Inside this directory, create subdirectories for each person you want to recognize and place their images in these subdirectories.

- **Generate Encodings**

  Run the script to generate face encodings and labels. This will create files necessary for training.

  **Note:** Ensure each image contains only one face; otherwise, only the first detected face will be encoded.

- **Train the Classifier**

  Train the face recognition classifier. This step will produce the trained model file.

### 3. Make Predictions

- **Prepare Test Images**

  Create a folder named `test-images` and place all the images you want to test in this folder.

- **Run Predictions**

  Predict faces in the test images using the trained model.

## License

This project is licensed under the MIT License.
