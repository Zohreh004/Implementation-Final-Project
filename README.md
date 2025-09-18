# 🖼️ Image Denoising using Higher Order Singular Value Decomposition (HOSVD)

This repository contains the final project for the **Image Processing** course at  
**Amirkabir University of Technology (Tehran Polytechnic)**.  
The project introduces an **HOSVD-based image denoising algorithm**, combining **tensor decomposition** and **machine learning** techniques.

---

## 📖 Overview

This project presents a simple yet effective method for image denoising that:

- Groups similar image patches into a 3D (grayscale) or 4D (color) tensor
- Applies **Higher Order Singular Value Decomposition (HOSVD)** to obtain data-driven bases
- Filters noise by thresholding the HOSVD coefficients
- Reconstructs the image by applying the inverse HOSVD transform and averaging overlapping patches
- Optionally applies a **Wiener filter (HOSVD2)** as a second refinement stage
- Combines **ResNet neural network** with **adaptive threshold prediction** to improve denoising quality
