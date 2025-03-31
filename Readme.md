# Deep Learning Atelier 2



**Developed by:** Amine Izougaghen  
**Supervised by:** Prof. EL ACHAAK Lotfi

![Project Badge](https://img.shields.io/badge/Deep%20Learning-PyTorch-blue)

## 📌 Overview

This project explores and implements various deep learning architectures for image classification tasks, including:
- Conventional CNNs
- Faster R-CNN (adapted)
- Fine-tuned pre-trained models (VGG16, AlexNet)
- Vision Transformers (ViT)

## Lab Report

This lab explored various deep learning architectures for image classification, highlighting their strengths, weaknesses, and practical implementation challenges.

---

## Part 1: CNNs, Faster R-CNN, and Fine-tuning

### CNN (Convolutional Neural Network)
- Designed and trained a basic CNN for MNIST classification.
- Learned layer composition: **convolutional → pooling → fully connected**.
- **Key takeaway**: CNNs efficiently capture spatial hierarchies, making them ideal for simple image tasks.

### Faster R-CNN (Adapted for MNIST)
- Repurposed an object detection model for classification.
- **Challenges:**
  - Complex setup compared to CNNs.
  - Required custom data formatting (target dictionaries).
- **Realization**: Overkill for MNIST—better suited for detection tasks.

### Fine-tuning Pre-trained Models
- Experimented with **VGG16** and **AlexNet** using transfer learning.
- **Strategy:** Froze early layers, retrained classifier head.
- **Results:** High accuracy with minimal training time.
- **Lesson:** Pre-trained models are powerful but require careful adaptation.

---

## Part 2: Vision Transformer (ViT)

### Implementation Challenges
- Built ViT from scratch:
  - **Image patching → embeddings → positional encoding**.
  - Implemented **multi-head self-attention**.
- **Performance:** Initially lagged behind CNNs, likely due to:
  - Hyperparameter sensitivity.
  - ViT’s hunger for larger datasets.

### Key Learnings
- Gained intuition for **self-attention** and transformer mechanics.
- ViTs show promise but require more tuning/data than CNNs for small-scale tasks.

---

## Conclusion
- **CNNs**: Simple, effective for basic tasks.
- **Faster R-CNN**: Powerful but unnecessarily complex for MNIST.
- **Fine-tuning**: Leveraging pre-trained models accelerates development.
- **ViTs**: Future potential, but need optimization for small datasets.

---


