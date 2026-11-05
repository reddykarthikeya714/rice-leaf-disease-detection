# Rice Leaf Disease Detection

A deep-learning image-classification project that explores identifying three rice leaf disease categories from images using a custom Convolutional Neural Network (CNN) and MobileNetV2 transfer learning.

## Project at a glance

| Item | Details |
|---|---|
| Problem type | Image classification |
| Domain | Agriculture |
| Classes | Leaf Smut, Brown Spot, Bacterial Leaf Blight |
| Dataset size described in notebook | 120 images |
| Image size | 128 × 128 |
| Models compared | Basic CNN and MobileNetV2 |

## Objective

Build and compare deep-learning approaches for classifying rice leaf images into the three categories represented in the dataset. The project demonstrates an end-to-end image-classification workflow, including visual exploration, preprocessing, model training, and evaluation.

## Dataset and exploration

The notebook describes a small dataset of 120 images across the three classes. The exploratory analysis counts images per class and displays sample images to inspect the visual patterns.

The image folder is expected to be available locally as `RiceLeaf Dataset`.

## Workflow

### 1. Image preprocessing
- Resize images to 128 × 128 pixels.
- Rescale pixel values by 1/255.
- Apply augmentation with rotation, zoom, and horizontal flipping.
- Use a 20% validation split.

### 2. Model development
- Build and train a basic CNN.
- Compare it with MobileNetV2 transfer learning using ImageNet weights.
- Freeze the MobileNetV2 base model during the described experiment.

### 3. Evaluation
- Generate classification reports and confusion matrices.
- Compare validation accuracy between the two approaches.

## Tools and technologies

Python · TensorFlow / Keras · MobileNetV2 · NumPy · Matplotlib · ImageDataGenerator

## Run locally

1. Clone this repository.
2. Place the `RiceLeaf Dataset` folder in the expected location, or update the notebook's dataset path.
3. Open the notebook in Jupyter Notebook, JupyterLab, or Google Colab.
4. Install the required libraries.
5. Run the notebook cells in order.

## Limitations

- The dataset is small (120 images), which limits confidence in generalization.
- The described experiment uses a validation split; an independent test set is needed for a stronger estimate of performance on unseen images.
- Training is described as 10 epochs, which may not be sufficient for convergence.
- No final performance score is stated here because a verified final result is not available.

## Future improvements

- Collect more images across different fields, lighting conditions, and disease stages.
- Keep a separate, unseen test set.
- Inspect class balance and image dimensions systematically.
- Tune training duration and model parameters.
- Test robustness on images captured outside the dataset environment.

---

*Portfolio project | Deep Learning · Computer Vision · Transfer Learning · Agriculture*
