# GAN-Based Medical Image Generation

This project implements Generative Adversarial Networks (GANs) using PyTorch to generate synthetic images, covering both synthetic 2D data and real-world medical imaging using the PathMNIST dataset.

##  Project Structure

### Part 1: 2D Data Distribution
-  GAN trained on sine wave samples
-  GAN trained on a noisy parametric curve:  
  `y = sin(2x) + 0.3cos(5x) + ε`
-  Architecture modifications (activation function, depth)
-  Visual comparison of generated vs. real data

### Part 2: Medical Image Synthesis – PathMNIST
-  DCGAN trained on pathology image data
-  Visual analysis of generated pathology samples
-  Generator and Discriminator loss tracking
-  Class-specific image generation using Conditional GAN (cGAN)

---

##  Folder Layout

gan-medical-image-generation/
│
├── part1_synthetic_gan/
│ ├── sine_wave_gan.ipynb
│ └── noisy_curve_gan.ipynb
│
├── part2_pathmnist_dcgan/
│ ├── Pathology_Image_Generation_with_cGAN.ipynb
│ └── figures/
│ ├── figure4_class_distribution.png
│ ├── figure5_dcgan_output.png
│ └── figure6_cgan_output.png
│
├── report/
│ └── GAN_Report.pdf # Optional if you want to include it
│
└── README.md

##  Requirements

- Python 3.8+
- PyTorch
- torchvision
- matplotlib
- medmnist

To install the required packages:
```bash
pip install torch torchvision matplotlib medmnist

