This repository contains the work for the AI for Healthcare project. The work combines foundational image processing concepts, CNN theory, and hands-on deep learning implementation using YOLOv8 for image classification.
The project is ongoing, and this submission documents the concepts learned and implementations completed up to the midterm stage.

**Week 1** – Foundations of AI for Healthcare

**Topics Covered:**
Introduction to AI applications in healthcare
Role of medical imaging in diagnosis and screening
Ethical considerations and limitations of AI in healthcare


**Week 2** -  Image Processing (Week 1 Practical)

**Notebook:** https://colab.research.google.com/drive/15Gr3UydbxL7EplYcpfUoBwJpph5vAWem?usp=sharing

**Concepts Implemented:**
Image representation and pixel manipulation
Grayscale conversion and thresholding
Basic filtering and preprocessing techniques
Understanding how preprocessing impacts downstream ML models

This stage helped build intuition for how raw medical images are prepared before being used in deep learning models.

**Week 3** – YOLOv8 Image Classification

**CNNs, Darknet, and YOLO (Theory)**

**Concepts Studied:**
Convolutional Neural Networks (CNNs)
ImageNet and transfer learning
Popular CNN architectures: AlexNet, VGG, ResNet, EfficientNet
Darknet framework and its role in early YOLO models
YOLO architecture and modes (Train, Val, Predict)

**Notebook:**https://colab.research.google.com/drive/1b-OztTpRLX8zbN3GvukA13IMnpq3ZU31?usp=sharing

**Objective:**
To gain practical exposure to YOLOv8 classification by training and evaluating a model on an image dataset.
Implementation Details

Model: YOLOv8 Nano Classification (yolov8n-cls)
Framework: Ultralytics YOLOv8
Platform: Google Colab (GPU)
Epochs: 10
Image Size: 224 × 224

**Dataset**
Explored: Skin Disease Dataset (Roboflow)- https://app.roboflow.com/cxrdataset/skin-ga5ww/ 
Implemented: CIFAR-10 (Ultralytics-supported)- https://www.cs.toronto.edu/~kriz/cifar.html

Due to technical issues with dataset structure and ZIP handling while using the Roboflow dataset in Colab, a standard dataset was used at this stage to correctly demonstrate the YOLOv8 training and inference workflow.

**Current Results** 
Training loss decreases consistently across epochs
Classification accuracy improves steadily
Successful inference on sample test images
Screenshots of training logs and prediction outputs are included in Result.pdf.

**Learnings So Far**
Fundamentals of image preprocessing
Working of CNNs in vision tasks
Practical understanding of YOLOv8 classification
Training, validation, and prediction workflows
Handling real-world issues with datasets, Colab, and GitHub

