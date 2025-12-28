# Convolutional Autoencoder – Fashion-MNIST

This repository contains a semester project for the course *Introduction to Deep Learning*.

The goal of the project is to design and evaluate a convolutional autoencoder
for image reconstruction on the Fashion-MNIST dataset, with a focus on the
influence of latent space size on reconstruction quality.

## Dataset

The Fashion-MNIST dataset is automatically downloaded using `torchvision` and
stored locally in the `data/` directory.
The dataset itself is not included in this repository.

## Model

The implemented model is a convolutional autoencoder consisting of:
- an encoder with convolutional layers and a fully connected latent representation,
- a decoder based on transposed convolutions.

Several latent space sizes were tested to analyze the trade-off between
compression and reconstruction quality.

## Experiments and Evaluation

The project includes:
- training and validation loss comparison (MSE),
- test loss evaluation,
- reconstruction visualizations,
- SSIM metric for structural similarity,
- error map visualization.

## How to run

Install dependencies:
```bash
pip install -r requirements.txt
```


Open the notebook:
```bash
jupyter notebook notebook/fashion_autoencoder.ipynb
```
