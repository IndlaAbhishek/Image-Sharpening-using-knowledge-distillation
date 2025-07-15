# Image Sharpening With Knowledge Distillation

The project aims to improve the sharpness and visual accuracy of low-quality images through a light, real-time model learned through **Knowledge Distillation**. An efficient high-performance teacher model (SwinIR-M) trains a small student CNN to replicate its sharpening ability while retaining rapid inference rates.

--- 

## Problem Statement

Compressed, downscaled, or lossy transformation images frequently lose edge details and sharpness. The current project focuses on repairing these images using a student-teacher distillation network, rendering the solution applicable to real-time and low-resource settings.

---

## System Overview

- **Teacher Model**: SwinIR-M (pretrained Transformer-based image restorer)
- **Student Model**: Lightweight CNN trained with L1, perceptual, and distillation loss
- **Training Data**: DIV2K (800 high-resolution images)
- **Evaluation Metrics**: SSIM, FPS (real-time readiness)

## Features

- Distillation of a large model to a small model
- Patch-based simulation of image degradation
- Paired training custom PyTorch DataLoader
- High sharpening accuracy (SSIM > 90%)
- Real-time inference speed (30–60 FPS on 1080p images)

---

## Tech Stack

- PyTorch
- torchvision, PIL, OpenCV
- VGG-based Perceptual Loss
- skimage (for SSIM)
- Google Colab (for training)

---

✨ Project by
- Indla Abhishek
- Male keerthan Reddy
- G Mahidhar
