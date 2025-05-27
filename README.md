

## Introduction

This repository contains the official source code for **Inter-Modality Feature Representation Learning-based Fusion Network for 3D Shape Defect Detection**.

## ABSTRACT
This paper presented a novel framework for defect detection in 3D shapes, addressing a gap in existing research that mainly focuses on 2D-based methods. We proposed an inter-modality feature representation learning and fusion based framework, combining RGB images, depth images, and point clouds to enhance defect detection in industrial manufacturing contexts. Our proposed framework consists of three key components: pre-trained feature extractors, the multi-level Adaptive Dual Modal Gated Fusion (ADMGF) module, and the inter-modality feature representation network. The design facilitates precise localization of anomalous regions by generating a combined anomaly map based on discrepancies between extracted and predicted multimodal representations. Experiments on the MVTec3D-AD and Eyecandies datasets showed significant improvements in performance over state-of-the-art methods.

## Requirement

- Ubuntu 18.04

## Environment

- Python >= 3.8

## Packages

- torch
- torchvision
- numpy
- opencv-python

For other required packages refere to requirement.txt file 

### Install pointnet2_ops_lib
```bash
pip install "git+git://github.com/erikwijmans/Pointnet2_PyTorch.git#egg=pointnet2_ops&subdirectory=pointnet2_ops_lib"
```

## RUN Model


## Dataset Download and Preprocessing

### Dataset

The **MVTec-3D AD dataset** can be downloaded from the [Official Website of MVTec-3D AD](https://www.mvtec.com/company/research/datasets/mvtec-3d-ad).

The **Eyecandies dataset** can be downloaded from the [Official Website of Eyecandies](https://eyecan-ai.github.io/eyecandies/).

After downloading, move the dataset to the `data` folder.

### Data Preprocessing

To run the preprocessing for background removal and resizing, run the following command:

```bash
python preprocess/preprocessing_mvtec3d.py
```

