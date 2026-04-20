# Tiny-Pest-Intelligence-Multi-Class-Detection-Recommendation-System
Tiny Pest Intelligence: AI framework using enhanced YOLOv11 with P2 layers and NWD loss to detect microscopic pests. Trained on Pest24, it assesses infestation severity and utilizes LLMs to deliver real-time, actionable crop management recommendations for precision agriculture.

Your README.md file is ready.

Tiny Pest Intelligence: Multi-Class Detection and Recommendation System
Overview
Tiny Pest Intelligence is an AI-powered framework designed to detect multiple types of agricultural pests and provide automated management support for farmers. The system enhances the YOLOv11 object detection model by incorporating a P2 high-resolution feature layer and Normalized Wasserstein Distance (NWD) loss to accurately identify microscopic and densely clustered pests that traditional models often miss.

Problem Statement
Traditional pest detection relies on manual visual inspection, which is time-consuming, error-prone, and often results in late-stage identification. Incorrect pest identification leads to the misuse of pesticides, increasing production costs and harming the environment. This project provides a scalable, automated solution for early-stage detection and precision agriculture.

Key Features

Multi-Class Detection: Identifies multiple pest species simultaneously within a single field image.


Small Object Optimization: Utilizes a P2 feature layer to capture fine spatial details of pests as small as 4-8 pixels.


Advanced Localization: Employs NWD loss to improve bounding box stability for tiny targets.


Severity Estimation: Analyzes pest density to categorize infestation levels as Low, Medium, or High.


Intelligent Recommendations: Integrates Large Language Models (LLMs) to provide tailored pest management strategies and control measures.


Real-Time Performance: Achieves an inference speed of 81 FPS, suitable for mobile and edge deployment.

Technical Architecture

Base Model: YOLOv11 (Ultralytics).


Feature Enhancement: Convolutional Block Attention Module (CBAM) to prioritize relevant image regions and mitigate noise.


Dataset: Trained on the Pest24 dataset, which contains 24 categories of pests collected from real agricultural fields.


Backend: PyTorch for model training and inference.


Web Interface: Flask-based application for image uploads and real-time result visualization.

Tech Stack

Language: Python 


Deep Learning: PyTorch, Ultralytics YOLO 


Image Processing: OpenCV, NumPy 


Web Framework: Flask 


Environment: Jupyter Notebook / VS Code 

Project Structure

App.py: The web application backend handling image processing and model inference.


Train.py: Script for model training, including CBAM injection and NWD loss implementation.


YOLOV11-p2.yaml: Model configuration file defining the backbone, P2 layers, and detection heads.


best.pt: The trained weights used for detection.

Results
The system demonstrates a robust balance between precision and recall, achieving approximately 81% convergence accuracy. It effectively distinguishes between diverse species even in complex backgrounds with varying lighting conditions.

Authors
K. Govardhan - 22HP1A4245 

B. Ankamma - 22HP1A4238 

V. Padmakanth - 22HP1A4253 


Project Guide: Mrs. D. Archana, Assistant Professor, Dept. of CSE (AI & ML) 

Acknowledgements
Developed at the Andhra Loyola Institute of Engineering and Technology (ALIET), Vijayawada, affiliated with JNTU Kakinada. This research was presented at the 5th International Conference on Advances in Science, Engineering & Technology (ICASET-2026).
