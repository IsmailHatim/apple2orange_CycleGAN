# CycleGAN Reimplementation: Apple2Orange

This repository contains a reimplementation of the CycleGAN paper, specifically trained and evaluated on the Apple2Orange dataset. The goal of the project is to explore unsupervised image-to-image translation using CycleGAN.

![CycleGAN Example](https://junyanz.github.io/CycleGAN/images/cyclegan_blogs.jpg)

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model](#model)
- [Implementation](#implementation)
- [Results](#results)
- [Usage](#usage)
- [Acknowledgments](#acknowledgments)

---

## Introduction
CycleGAN is a framework for unpaired image-to-image translation. Unlike paired datasets, CycleGAN learns to transform images between two domains (e.g., apples and oranges) without requiring one-to-one correspondence between images in these domains.

For more details, refer to the original [CycleGAN paper](https://arxiv.org/abs/1703.10593).

---

## Dataset
The dataset used for this implementation is Apple2Orange, a benchmark dataset commonly used for image-to-image translation tasks.

---

## Model
The CycleGAN framework consists of:
1. Two generators \( G: X \rightarrow Y \) and \( G: Y \rightarrow X \)
2. Two discriminators \( D_X \) and \( D_Y \), ensuring the generated images are indistinguishable from real ones.

Key Losses:
- Adversarial Loss
- Cycle Consistency Loss
- Identity Loss

---

## Implementation
This implementation is written in Pytorch, leveraging the following frameworks:
- NumPy
- Matplotlib for visualization

---

## Results
You can see the results at the end of the Jupyter notebook.
---

## Usage
### Prerequisites
Install the necessary dependencies:
```bash
pip install -r requirements.txt
```

### Training
To train the CycleGAN model on Apple2Orange:

Run the training cell in the Jupyter notebook, you can save your model as training checkpoints.

### Evaluation
To generate images:

You can run generate cell in the Jupyter notebook.

---

## Acknowledgments
This work is based on the CycleGAN implementation by [Jun-Yan Zhu et al.](https://github.com/junyanz/CycleGAN).

---
