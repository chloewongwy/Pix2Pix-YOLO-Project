# Image-to-Image Translation and YOLO Adaptation

This repository contains the implementation and report for a **COMP4423 Computer Vision project** on **Image-to-Image Translation using Pix2Pix GAN** and **YOLOv5 adaptation**.  

## 📅 Project Info  
- Developed: May 2025  

---

## 📂 Project Structure

```
src/
│── main.ipynb                # Main notebook implementing Pix2Pix GAN and YOLO adaptation
│── input_file/               # Input files for testing and evaluation
│    ├── predicted_images/    # Generated images from Pix2Pix
│    ├── last_.pt             # Saved model checkpoint
│    ├── test_image.png       # Example test input
│── custom model train/       # Custom YOLO training files and configurations
report.pdf                    # Detailed project report with methods and results
.gitattributes                # Manage file types and behaviors in a Git repository
CV_Project.pdf                # Assignment specification
```

---

## 📌 Assignment Tasks

This project followed the COMP4423 Assignment requirements:

- **Task 1 (10 marks):** Build the necessary datasets for Pix2Pix GAN.  
- **Task 2 (10 marks):** Design and implement the Generator (U-Net) and Discriminator (PatchGAN).  
- **Task 3 (20 marks):** Implement the training pipeline with adversarial + L1 loss and optimization.  
- **Task 4 (10 marks):** Evaluate the trained generator on unseen test images, analyze performance, and identify improvements.  
- **Task 5 (10 marks):** Apply model adaptation/fine-tuning techniques to improve a pretrained YOLO model on Pix2Pix-generated images (e.g., TTA, custom fine-tuning).  
- **Task 6 (10 marks):** Evaluate the adapted YOLO model, including strategies for generating labels for unlabeled data.  
- **Task 7 (30 marks):** Prepare the final report summarizing approach, methodology, results, and insights.  

---

## 🚀 Features

- **Pix2Pix GAN (Image-to-Image Translation)**  
  - Dataset preparation (Cityscapes dataset)  
  - U-Net Generator & PatchGAN Discriminator  
  - Training with adversarial + L1 loss  
  - Visualization of generated images  

- **Evaluation of Pix2Pix**  
  - SSIM, L1 Loss, qualitative visualizations  

- **YOLO Adaptation**  
  - Apply pretrained YOLOv5 to Pix2Pix outputs  
  - Fine-tune with car labels & augmentation techniques  
  - Evaluation with IoU, precision, recall, F1, and mAP  

---

## 📖 Report

A complete explanation of methodology, training progress, results, and evaluation is available in [`report.pdf`](./report.pdf).

---

## 🛠 Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/chloewongwy/Pix2Pix-YOLO-Project.git
   cd Pix2Pix-YOLO-Project
   ```

---

## ▶️ Usage

Run the main notebook:
```bash
jupyter notebook src/main.ipynb
```

- **Pix2Pix Training:**  
  Training is configured inside `main.ipynb`. Checkpoints are saved in `input_file/last_.pt`.  

- **YOLO Adaptation:**  
  Custom YOLO training and evaluation scripts are inside `custom model train/`.  

---

## 📌 Requirements

- Python 3.8+  
- PyTorch / TensorFlow  
- torchvision  
- numpy, matplotlib, pandas  
- Jupyter Notebook  
- ultralytics (YOLOv5)  

---

## 📜 Acknowledgements

- Dataset: [Cityscapes Dataset](http://efrosgans.eecs.berkeley.edu/pix2pix/datasets/)  
---
