# Deep Learning Project for Environmental Sound Classification

This repository contains a description of my deep learning project on environmental sound classification using the ESC-50 dataset (https://github.com/karolpiczak/ESC-50).

The project explores different audio representations and data augmentation strategies, and compares their impact on classification performance using convolutional neural networks (CNNs). The work was completed as part of an undergraduate machine learning mini-project (UCL PHAS0056 Practical Machine Learning for Physicists).

## Project Overview

Environmental sound classification is a challenging task due to background noise, short-duration events, and high intra-class variability.

In this project, the following aspects were investigated:

* CNN-based classification of environmental sounds

* Raw audio vs Mel spectrogram input representations

* The effect of different data augmentation techniques on model performance

Experiments were conducted on both the full 50-class ESC-50 task, and a simplified 5 super-category classification task.

## Methods

### Data

Dataset: ESC-50 (50 environmental sound classes)

* Train/test split: 80% / 20%

### Preprocessing

* Audio resampling and fixed-length padding/truncation

* Mel spectrogram extraction using Librosa

* Normalisation and reshaping for CNN input

### Data Augmentation

* Pitch shifting

* Time stretching

* White noise and pink noise injection

* Combined augmentation strategies


### Evaluation

* Classification accuracy

* Confusion matrices

* Per-class performance analysis

### Results (Summary)

* Data augmentation improved classification accuracy by ~15% compared to baseline models

* Mel spectrogram representations consistently outperformed raw waveform inputs

* Best performance was achieved using combined augmentation strategies

* Raw audio models were more sensitive to noise and required stronger regularisation

* More detailed results, figures, and discussion can be found in the project report.


## Dataset Setup

The ESC-50 dataset is not included in this repository.

To run the notebook:

* Download the ESC-50 dataset from the official source: https://github.com/karolpiczak/ESC-50

* Place the audio and metadata files in a local data/ directory

* Update file paths in the notebook if needed

## Notes

This project was completed as part of undergraduate coursework and focuses on experimentation and analysis rather than production-level optimisation. The code is provided for demonstration purposes.
