
# Part 2 - CNN Computer Vision Project

## Problem Statement
This project builds a Convolutional Neural Network (CNN) model for image classification using a synthetic manufacturing defect dataset.

The objective is to classify product surface images into one of four categories:

- normal
- scratch
- dent
- stain

---

# Task 1: Problem Identification

## Problem Type: Image Classification

This dataset represents an image classification problem because:

- Each image belongs to exactly one class
- The goal is to predict a single label for every image
- There are no bounding boxes or segmentation masks
- Images are grouped into folders by category

Classes:
- normal → no defects
- scratch → scratch marks
- dent → circular dents
- stain → stain-like defects

---

# Task 2: Dataset Exploration

## Dataset Details

The dataset contains four image classes:

| Class | Description |
|------|------|
| normal | Surface without defect |
| scratch | Surface with scratches |
| dent | Surface with dents |
| stain | Surface with stains |

---

# Task 3: Image Preprocessing

The following preprocessing steps were applied:

- Resized all images to 128x128
- Normalized pixel values to range [0,1]
- Split dataset into training and testing sets
- Applied image augmentation:
  - rotation
  - zoom
  - horizontal flip

---

# Task 4: CNN Model Architecture

The CNN model includes:

1. Convolution Layers
2. ReLU Activation
3. MaxPooling Layers
4. Flatten Layer
5. Dense Fully Connected Layer
6. Softmax Output Layer

---

# Task 5: Model Training and Evaluation

Evaluation metrics:
- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss
- Test Accuracy
- Confusion Matrix
- Sample Predictions

---

# Task 6: CNN Concept Explanation

## What is Convolution?

Convolution is a mathematical operation where filters slide over an image to detect important patterns such as:
- edges
- textures
- shapes

## Why is Pooling Used?

Pooling reduces the size of feature maps.

Benefits:
- Reduces computation
- Prevents overfitting
- Keeps important features

## Why is ReLU Commonly Used?

ReLU (Rectified Linear Unit):

f(x) = max(0,x)

Advantages:
- Fast computation
- Helps deep networks learn better
- Prevents vanishing gradient problems

## Why are CNNs Better than Feed-Forward Networks for Images?

CNNs are better because:
- They preserve spatial information
- Require fewer parameters
- Automatically learn image features
- Work efficiently on image patterns

---

# Task 7: Business Use Case Mapping

## Manufacturing Quality Inspection

This solution can be used in manufacturing industries for automated defect detection.

Applications:
- Detect scratches on metal surfaces
- Identify damaged products
- Reduce manual inspection
- Improve production quality
- Increase inspection speed

Industries:
- Automotive
- Electronics
- Steel manufacturing
- Consumer goods

---

# Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

# How to Run

## Install Requirements

```bash
pip install -r requirements.txt
```

## Run Notebook

```bash
jupyter notebook
```
