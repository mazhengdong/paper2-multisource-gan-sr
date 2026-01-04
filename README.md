# GAN-based Multi-source Image Super-Resolution with Multi-constraint Learning (Paper 2)

This repository corresponds to the second first-author research project on **GAN-based multi-source image super-resolution**, focusing on incorporating **multi-source physical and auxiliary constraints** to improve reconstruction accuracy and spatial consistency.

## Overview

High-resolution image reconstruction from coarse-resolution multi-source inputs remains challenging due to spatial heterogeneity and complex nonlinear relationships. This work proposes a **deep learning–based multi-source super-resolution framework** that integrates adversarial learning with auxiliary constraint information to enhance fine-scale image reconstruction.

## Dataset

* Multi-source geospatial datasets (Dataset B)
* Coarse-resolution inputs combined with auxiliary constraint variables
* Target resolution: coarse (~10–50 km) → fine (~500 m)
* Temporal split for training and testing to ensure generalization

> Note: Original datasets are not publicly released due to data usage policies.

## Method

* GAN-based generator–discriminator architecture
* Multi-scale feature extraction using inception-style convolution blocks
* Integration of multi-source auxiliary constraints (e.g., meteorological and surface-related variables)
* Spatial and channel attention mechanisms to enhance feature representation
* Joint optimization with adversarial loss and reconstruction-based objectives

## Experiments

* Systematic evaluation of different input-variable combinations
* Comparison with baseline and unconstrained models
* Quantitative metrics include accuracy-related indicators and distributional divergence measures
* Qualitative spatial pattern analysis to assess reconstruction consistency

## Implementation

The core model and training pipeline are implemented in PyTorch and shared in the following repository:

* **Core implementation**: [https://github.com/mazhengdong/dl-multisource-super-resolution-core.git](https://github.com/mazhengdong/dl-multisource-super-resolution-core.git)

This repository focuses on **project-level configuration, experimental design, and result interpretation** corresponding to Paper 2.

## Results

Experimental results demonstrate that incorporating multi-source constraints significantly improves reconstruction accuracy and spatial consistency compared to baseline GAN-based super-resolution approaches.

## Author

* **First Author & Core Algorithm Developer**: Mazhengdong

## Citation

If you find this work useful, please cite the corresponding paper.


