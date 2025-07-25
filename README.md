# Single Image Dehazing using EENet 

This project implements a deep learning-based solution for **single image dehazing** using the lightweight and efficient **EENet** architecture. The model is trained and evaluated using the **S‑Dust dataset** from [agriscapes-dataset.com](https://agriscapes-dataset.com/s-dust/), which contains real-world images of agricultural fields affected by dust and haze.

---

## Table of Contents

- [Overview](#overview)
- [Model Architecture](#model-architecture)
- [Dataset - S-Dust](#dataset---s-dust)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Project Structure](#project-structure)
- [References](#references)
- [Citation](#citation)
- [Contact](#contact)

---

## Overview

Real-world applications in agriculture, autonomous driving, and remote sensing suffer from the presence of haze or dust in captured images. This project aims to remove that haze using a computationally efficient neural network—**EENet**—and improve image clarity for downstream vision tasks.

---

## Model Architecture

**EENet** (Effective and Efficient Network) is designed to:
- Be **lightweight (~74K parameters)**
- Utilize **EED blocks** (Effective and Efficient Dilation) to capture multi-scale context
- Be deployable on edge devices with limited compute resources

The model follows an encoder-decoder design with dilated convolutional layers in the bottleneck for enhanced receptive field.

---

## Dataset - S‑Dust

This project uses the **S-Dust dataset**, the **first publicly available benchmark for pixel-wise segmentation and enhancement of dust in agriculture images**.

### Highlights:

- 963+ annotated RGB images (field crop scenes)
- Binary segmentation masks (dust vs. background)
- Diverse dust intensities and environmental conditions

