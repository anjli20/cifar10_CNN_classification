# Image Classification on CIFAR-10 using Advanced CNN

CIFAR-10 image classification using a deep Convolutional Neural Network built from scratch in TensorFlow/Keras.
Achieves **86% test accuracy** with Batch Normalisation, Dropout, Data Augmentation, and adaptive learning rate 
scheduling.

## Results
 Model - **CNN**

 Test Accuracy - **86.06%** 


## Techniques Used
- **3-Block CNN Architecture** — Stacked Conv2D layers with 32 → 64 → 128 filters
- **Batch Normalisation** — After every convolutional layer for stable training
- **Dropout** — Rates of 0.25, 0.40, and 0.50 to prevent overfitting
- **Data Augmentation** — Random flips, rotations, shifts, and zooms
- **ReduceLROnPlateau** — Adaptive learning rate halved on validation plateau
- **Early Stopping** — Stops training and restores best weights automatically
- **Model Checkpointing** — Saves the best model during training

## Dataset
[CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) — 60,000 colour images (32×32) across 10 classes, loaded directly via `tensorflow.keras.datasets`.

**Classes:** airplane · automobile · bird · cat · deer · dog · frog · horse · ship · truck
