# Pix2Pix-GAN-Image-to-Image-Translation-System
Implemented a Pix2Pix Conditional GAN using a U-Net generator and PatchGAN discriminator to perform image-to-image translation on paired datasets, focusing on structural preservation and robust model evaluation.


Pix2Pix GAN – Image-to-Image Translation System

(Computer Vision & Deep Learning Project)

📌 Project Overview

This project implements a Pix2Pix Conditional GAN to perform image-to-image translation using paired data. A U-Net based generator and PatchGAN discriminator were trained to learn structured visual transformations while preserving fine-grained details.

🎯 Problem Statement

Image-to-image translation is a core problem in computer vision, especially in domains like medical imaging, where structural consistency and feature preservation are critical. This project explores supervised GANs for learning complex visual mappings.

🧠 Technical Approach

Generator: U-Net architecture with skip connections for spatial detail preservation

Discriminator: PatchGAN for local texture realism

Loss Function: Adversarial loss + L1 reconstruction loss (λ = 100)

Training: Stable GAN training with dropout, batch normalization, and learning rate scheduling

📊 Dataset & Preprocessing

Used 5,000 paired images (train/val/test split: 70/15/15)

Images resized to 256×256, normalized to [-1, 1]

Applied augmentation (horizontal flips) to improve generalization

📈 Results & Evaluation

Model performance was evaluated using both qualitative and quantitative metrics:

SSIM: 0.88 (structural similarity)

PSNR: 28.4 dB

MAE: 0.05
Results show strong structural preservation and visually consistent translations.

🧪 Key Learnings

Stabilizing GAN training and preventing mode collapse

Designing scalable evaluation pipelines for generative models

Applying CNN architectures (U-Net) commonly used in biomedical imaging

Understanding practical trade-offs in deep learning model optimization

🛠 Tech Stack

Language: Python

Framework: PyTorch

Libraries: NumPy, torchvision, scikit-image, Matplotlib

Hardware: NVIDIA GPU (Kaggle environment)

🔬 Relevance to Healthcare & Pharma

The same Pix2Pix architecture can be applied to:

Medical image modality translation (e.g., CT ↔ MRI)

Image enhancement and denoising

Synthetic data generation for healthcare ML models
