# Rice Leaf Disease Detection

A deep-learning image-classification project comparing a custom Convolutional Neural Network (CNN) with MobileNetV2 to classify rice leaf images.

## Classes
- Leaf Smut
- Brown Spot
- Bacterial Leaf Blight

## Approach
- Explore class distribution and sample images.
- Resize images to **128 × 128** and rescale pixel values.
- Apply data augmentation using rotation, zoom, and horizontal flipping.
- Train a basic CNN and compare it with MobileNetV2 transfer learning.
- Evaluate using classification reports, confusion matrices, and validation accuracy.

## Dataset
The notebook describes **120 images** across the three classes. The dataset folder is expected to be named `RiceLeaf Dataset`.

## Technologies
Python · TensorFlow / Keras · MobileNetV2 · NumPy · Matplotlib

## Key concepts
Image Preprocessing · Data Augmentation · CNN · Transfer Learning · Image Classification · Model Evaluation

*The dataset is small, so performance should be validated on a larger, independent test set before drawing conclusions about real-world accuracy.*
