# NYCU Computer Vision 2025 Spring HW4

StudentID: 110550142  
Name:黃芷柔

## Introduction
In this project, we tackle the joint deraining and desnowing task using a pure vision-based model, without any pretrained weights or external datasets. Our approach is based on PromptIR, a prompt- guided restoration framework originally designed to adaptively inject learned priors into the reconstruction process. To reduce training resource consumption and accelerate convergence, we simplify the original architecture by reducing the number of prompt injection layers and decreasing overall model depth.
We implement the entire training and evaluation pipeline using PyTorch, and adopt PSNR as the primary evaluation metric.


## How to install
You can run this project directly in your browser using Google Colab. No local setup is needed.

Steps:
Click the badge above to open the notebook in Google Colab.  

Run all cells in the notebook to install dependencies, train, and evaluate the model.  

📦 All required packages will be installed automatically in the notebook.  

⚠️ Make sure you are using a GPU runtime by going to

   `Runtime > Change runtime type > Hardware accelerator > GPU`


## Performance snapshot

```
PSNR: 26.48(private)/26.85(public)
Backbone	PromptIR-like  
Training Epochs	10
Dataset	1600 images per types,256*256 png

