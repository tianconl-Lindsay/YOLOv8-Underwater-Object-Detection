# YOLOv8 Underwater Object Detection

This repository contains the report and related images for a course project on **underwater object detection using YOLOv8**. No executable code is included—this is a documentation and visualization repository for learning purposes.

## Project Information

- **Course:** Machine Learning and Deep Learning  
- **University:** Dalian University of Technology  
- **Department:** School of Software  
- **Major:** Software Engineering  
- **Student:** Tiancong Li  
- **Student ID:** 20212241276  
- **Instructor:** Fangming Zhong  
- **Completion Date:** June 20, 2024  

## Project Description

Underwater object detection is a challenging task due to light attenuation, scattering, and absorption in water, which degrade image quality and make object features difficult to extract. Additionally, underwater creatures vary greatly in shape, color, and size, adding complexity to recognition.  

This project uses **YOLOv8** for detecting underwater objects such as starfish, sea urchins, scallops, and sea cucumbers. YOLOv8 was chosen for its high efficiency, accuracy, and support for deployment on resource-limited devices.

### Key Steps:

1. **Data Preprocessing:**  
   - Color correction and enhancement using green channel adjustment and gray-world algorithm  
   - Image sharpening with unsharp mask  
   - Fusion of images using PCA to improve contrast and details

2. **Model Training:**  
   - Trained with `yolov8n.pt` weights on 2,374 preprocessed images  
   - 90% images used for training

3. **Evaluation:**  
   - Overall test accuracy: **81.25%**  
   - Class-specific accuracies:  
     - Starfish: 78.26%  
     - Sea urchin: 90.32%  
     - Sea cucumber: 16.67%  
     - Scallop: 88%

4. **Results Visualization:**  
   - Confusion matrix, precision-recall curves, and sample detection images included in `images/` folder

## Folder Structure

- `docs/` – Contains the full project report  
- `images/` – Contains preprocessed images and visualizations of model evaluation  
- `dataset_info/` – (Optional) Description of datasets used  

## Note

This repository is **for documentation and educational purposes only**. No code is provided. Images and reports illustrate the workflow, preprocessing steps, and evaluation results of the YOLOv8 underwater object detection project.

