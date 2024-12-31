# SCT_ML_04
Hand Gesture Recognition

This project implements a hand gesture recognition system that identifies and classifies different hand gestures from images or video data. It can be used for intuitive human-computer interaction and gesture-based control systems.

Features

Classifies multiple hand gestures such as "Thumbs Up," "Palm," "Fist," "Peace," and "Okay."

Supports real-time gesture recognition using a webcam.

Provides a simple Convolutional Neural Network (CNN) architecture.

Includes data preprocessing with image augmentation for robust training.

Requirements

Python Libraries:

TensorFlow

NumPy

OpenCV

Matplotlib (optional for visualization)

Install the required packages using:

pip install tensorflow opencv-python numpy matplotlib

Dataset

The dataset should consist of images for each gesture category organized into separate folders.

Example:

path_to_hand_gesture_dataset/
├── Thumbs_Up/
├── Palm/
├── Fist/
├── Peace/
├── Okay/

You can use an existing dataset or collect your own using a webcam.

How to Run

Preprocess Data:

Place your dataset in the path_to_hand_gesture_dataset directory.

The script will automatically resize and normalize the images.

Train the Model:

Run the script to train the model using:

python hand_gesture_recognition.py

The model will be saved as hand_gesture_model.h5 after training.

Real-Time Gesture Recognition:

Ensure you have a webcam connected.

Run the script and the model will predict gestures in real-time.

Model Details

The model consists of:

Convolutional Layers: Extract spatial features.

Max Pooling Layers: Reduce dimensionality.

Dense Layers: For classification of gestures.

It is trained using categorical crossentropy loss and the Adam optimizer for 20 epochs.

Example Output

During real-time gesture recognition, the model will display:

The webcam feed with the detected gesture label overlaid.

Predictions updated in real-time as gestures change.

Limitations

Accuracy depends on the quality and diversity of the training dataset.

Lighting conditions and background noise may affect performance.

Future Improvements

Use a pretrained CNN (e.g., ResNet) for better feature extraction.

Add dynamic gesture recognition for video sequences using RNNs or 3D-CNNs.

Implement hand segmentation for more robust detection.

License

This project is open-source and available under the MIT License.

Feel free to contribute or raise issues for improvement!

