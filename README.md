# MNIST Hyperparameter Tuning

simple project that uses Keras Tuner to find a fully connected neural network configuration for recognizing handwritten digits.

## Overview

- Uses MNIST with 50,000 training, 10,000 validation, and 10,000 test images.
- Tunes network depth, hidden layer widths, activation, and Adam optimizer settings.
- Runs 20 RandomSearch trials, selecting the best configuration by validation accuracy.
- Trains the selected configuration, plots training and validation loss, and evaluates test performance.

## Results

The saved run achieved **97.40% best search validation accuracy** and **96.97% final test accuracy**. Results can vary between runs because the split and training are not seeded.

## Run

Use Python 3.11 and install the dependencies:

```bash
python -m pip install -r requirements.txt
```

Open [mnist_tuning.ipynb](mnist_tuning.ipynb) in a Jupyter-compatible editor, select the Python environment, and run the cells in order.
