# Handwritten Digit Recognition (CNN)

A convolutional neural network trained on MNIST to classify handwritten digits (0-9), with additional testing on my own handwritten digit photos.

## Overview

- **Data**: MNIST, 28x28 grayscale images, extended with a color-inverted copy for robustness
- **Model**: Small CNN (2x Conv2D + MaxPooling + Dense) built with TensorFlow/Keras
- **Result**: ~98.4% test accuracy
- **Extra check**: model is also run on a handful of digits I painted myself (`MeineTestBilder28x28/`), to see how it holds up on real, non-MNIST handwriting

## Project structure

```
digit_recognition_cnn.ipynb   # data loading, training, evaluation, own-image test
MeineTestBilder28x28/         # my own handwritten digit photos, sorted by label
```

## Running it

```
pip install -r requirements.txt
```

Then open `digit_recognition_cnn.ipynb`. It expects the MNIST CSV files (`mnist_train.csv`, `mnist_test.csv`, e.g. from [Kaggle](https://www.kaggle.com/datasets/oddrationale/mnist-in-csv)) in a `28x28 dataset/` folder next to the notebook.
