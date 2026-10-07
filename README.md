# Cat and Dog Image Classifier

## Overview
Convolutional Neural Network built with TensorFlow/Keras to classify photos of cats and dogs.

**freeCodeCamp:** Machine Learning with Python Certification — [certification page](https://www.freecodecamp.org/certification/fcc-ec5175fa-1c9f-4a8e-ae70-0f191f3a5883/machine-learning-with-python)

## What the project covers
- Loading and exploring the cats vs. dogs image dataset
- Image visualization with Matplotlib
- Data augmentation (rotation, shift, flip, zoom)
- CNN architecture: `Conv2D` → `MaxPooling2D` × 3, `Dropout`, `Flatten`, `Dense`
- Training with `ImageDataGenerator` (train / validation splits)
- Training vs. validation accuracy & loss curves
- Predicting labels for the unseen test set

## Model architecture
```
Conv2D(32) → MaxPooling2D
Conv2D(64) → MaxPooling2D
Conv2D(128) → MaxPooling2D → Dropout(0.2)
Flatten → Dense(512) → Dropout(0.5) → Dense(1, sigmoid)
```
Optimizer: `adam` · Loss: `binary_crossentropy` · Image size: 150×150 · Epochs: 20

## How to run
Open `solution.ipynb` in [Google Colab](https://colab.research.google.com/) and run all cells.
The dataset is downloaded automatically from freeCodeCamp's CDN.

## Result
Passed the freeCodeCamp challenge (>= 63% of test images identified correctly).

