# Rice Leaf Disease Detection

A deep-learning image classification project that identifies three rice leaf diseases from images:

- Leaf Smut
- Brown Spot
- Bacterial Leaf Blight

## Project Objective

Build and compare convolutional neural network approaches for classifying rice leaf images into the three disease categories.

## Dataset

The notebook describes a small dataset containing 120 images across the three classes. The image folder is expected to be available locally as `RiceLeaf Dataset`.

## Workflow

1. **Exploratory Data Analysis**
   - Count images in each class.
   - Display sample images from each category.
2. **Image Preprocessing**
   - Resize images to 128 × 128.
   - Rescale pixel values by 1/255.
   - Apply data augmentation: rotation, zoom, and horizontal flipping.
   - Use a 20% validation split.
3. **Model Development**
   - Train a basic CNN.
   - Compare it with MobileNetV2 transfer learning using ImageNet weights and a frozen base model.
4. **Evaluation**
   - Review classification reports and confusion matrices.
   - Compare validation accuracy.

## Technologies

- Python
- TensorFlow / Keras
- MobileNetV2
- NumPy
- Matplotlib
- ImageDataGenerator

## Important Notes and Limitations

- The notebook uses a relatively small dataset (120 images), so results may not generalize to new field conditions.
- The experiments use a validation split; an independent test set would provide a stronger estimate of performance on unseen images.
- The notebook trains for 10 epochs, which may not be sufficient for full convergence.
- No performance score is stated here because a verified final result is not available in the project summary.
- The dataset folder must be placed in the expected location or the notebook's data path must be updated.

## How to Run

1. Clone or download this repository.
2. Place the `RiceLeaf Dataset` folder in the location expected by the notebook.
3. Open the notebook in Jupyter Notebook, JupyterLab, or Google Colab.
4. Install the required Python libraries if they are not already available.
5. Run the cells in order.

## Future Improvements

- Add a separate unseen test dataset.
- Expand the dataset with more images and varied capture conditions.
- Inspect class balance and image dimensions.
- Tune training duration and model parameters.
- Evaluate robustness on images captured outside the training environment.

---
**Project:** Rice Leaf Disease Detection  
**Focus:** Deep Learning · Image Classification · Transfer Learning
