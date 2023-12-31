# Improved EEG-Based Driver Drowsiness Recognition

This repository contains an improved implementation of the "InterpretableCNN" model proposed in the paper "EEG-Based Cross-Subject Driver Drowsiness Recognition With an Interpretable Convolutional Neural Network" by J. Cui, Z. Lan, O. Sourina, and W. Müller-Wittig. The improvements focus on enhancing the accuracy of the original model.

If you find this code useful for your work, please consider citing the original paper:

J. Cui, Z. Lan, O. Sourina and W. Müller-Wittig, "EEG-Based Cross-Subject Driver Drowsiness Recognition With an Interpretable Convolutional Neural Network," in IEEE Transactions on Neural Networks and Learning Systems, doi: 10.1109/TNNLS.2022.3147208.


[Paper Link](https://ieeexplore.ieee.org/document/9714736)

## Project Overview

The project is implemented in Python 3.6.6 and includes three main code files:

1. **InterpretableCNN.py**: Contains the implementation of the improved InterpretableCNN model. Required library: torch.

2. **LeaveOneOut_acc.py**: Implements the leave-one-subject-out method to calculate classification accuracies. This requires a CUDA-supported GPU. Required libraries: torch, scipy, numpy, sklearn.

3. **VisTechnique.py**: Contains a novel visualization technique proposed in the paper. It also requires a CUDA-supported GPU. Required libraries: torch, scipy, numpy, matplotlib, mne.

## Dataset

The processed dataset used in this project is available on Figshare: [EEG Driver Drowsiness Dataset](https://figshare.com/articles/dataset/EEG_driver_drowsiness_dataset/14273687)

## Usage

1. **InterpretableCNN.py**: Run this file to train and test the improved InterpretableCNN model.

2. **LeaveOneOut_acc.py**: Execute this file to apply the leave-one-subject-out method for classification accuracies.

3. **VisTechnique.py**: Run this file to visualize the results using the proposed technique. Note: There may be Deprecation Warnings for mne library version v0.19.2; it has been tested and works perfectly with v0.18.

## Contact

For any issues or inquiries, please contact Dr. Cui Jian at cuij0006@ntu.edu.sg.

## Known Issue

The file **VisTechnique.py** has been tested on mne library versions v0.18 and v0.19.2. It works perfectly for v0.18, while there may be some Deprecation Warnings for v0.19.2. Ensure compatibility with the specified library versions to avoid potential issues.
