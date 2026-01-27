**AI-VISION IN HEALTHCARE- WiDS 5.0**
_________________________________________________________________________________________________________________________________________________________________________________

This repository contains the work for the AI for Healthcare project. The work combines foundational image processing concepts, CNN theory, and hands-on deep learning implementation using YOLOv8 for image classification.

**Project Objectives:**
Understand the role of AI in healthcare, especially medical imaging,
Learn digital image processing fundamentals,
Study CNN architectures and YOLO framework,
Implement YOLOv8 for image classification,
Gain exposure to real-world healthcare datasets,
Understand ethical, technical, and practical challenges in healthcare AI

**Week 1 – Foundations of AI for Healthcare**

**Topics Covered:**
Applications of AI in healthcare,
Importance of medical imaging in diagnosis and screening,
Types of healthcare and medical imaging reports,
Ethical considerations and limitations of AI in healthcare

**Key Learnings:**
Differences between clinical, radiology, pathology, and laboratory reports,
Structure of a medical imaging report (patient info, findings, impression, etc.),
Importance of accuracy, fairness, and explainability in healthcare AI systems

**Week 2 - Image Processing (Week 1 Practical)**

Notebook: https://colab.research.google.com/drive/15Gr3UydbxL7EplYcpfUoBwJpph5vAWem?usp=sharing

Concepts Implemented: Image representation and pixel manipulation, Grayscale conversion and thresholding, Basic filtering and preprocessing techniques, Understanding how preprocessing impacts downstream ML models

**Key Learnings**
How raw medical images are prepared before model training,
Why preprocessing strongly impacts model performance,
Differences between bilinear and bicubic interpolation,
Why HSV is often preferred over RGB for color-based analysis.

This stage built strong intuition about how computers “see” images.

**Week 3 – YOLOv8 Image Classification**

**CNNs, Darknet, and YOLO (Theory)**
Concepts Studied: Convolutional Neural Networks (CNNs), ImageNet and transfer learning, Popular CNN architectures: AlexNet, VGG, ResNet, EfficientNet Darknet framework and its role in early YOLO models, YOLO architecture and modes (Train, Val, Predict).

**Notebook:** https://colab.research.google.com/drive/1b-OztTpRLX8zbN3GvukA13IMnpq3ZU31?usp=sharing

Objective: To gain practical exposure to YOLOv8 classification by training and evaluating a model on an image dataset.

**Implementation Details**

Model: YOLOv8 Nano Classification (yolov8n-cls), Framework: Ultralytics YOLOv8, Platform: Google Colab (GPU), Epochs: 10, Image Size: 224 × 224

**Dataset:** Explored: Skin Disease Dataset (Roboflow)- https://app.roboflow.com/cxrdataset/skin-ga5ww/ Implemented: CIFAR-10 (Ultralytics-supported)- https://www.cs.toronto.edu/~kriz/cifar.html

Due to technical issues with dataset structure and ZIP handling while using the Roboflow dataset in Colab, a standard dataset was used at this stage to correctly demonstrate the YOLOv8 training and inference workflow.

Current Results: Training loss decreases consistently across epochs Classification accuracy improves steadily Successful inference on sample test images Screenshots of training logs and prediction outputs are included in Result.pdf.

**Week 4 – Automated Detection of Tumor-Infiltrating Lymphocytes**
**Objective:**
Develop an AI-based pipeline to automatically detect lymphocytes and plasma cells in breast cancer histopathology images using YOLOv8, aligned with the TIGER Grand Challenge.

**Dataset:** TIGER WSIRois Dataset (Roboflow)

Histopathology image patches with bounding box annotations

**Approach:**
Converted COCO annotations to YOLO format,
Patch-based training with resized images (512 × 512),
YOLOv8 object detection with pretrained backbone.

**Challenges Addressed:**
Small object detection,
Stain variability,
Class imbalance,
Overfitting risks in medical datasets.

**Outcome:**
This task provided real-world exposure to clinical AI workflows and demonstrated how object detection models can assist pathologists by enabling faster, consistent, and scalable TIL assessment.

**Key Learnings from the Project:**
Understanding of AI applications in healthcare and medical imaging,
Strong foundation in digital image processing,
Theoretical and practical knowledge of CNNs and YOLO architectures,
Experience in classification vs object detection workflows,
Handling real-world medical datasets and annotation formats,
Appreciation of small-object detection challenges in histopathology,
Awareness of ethical responsibility and reliability requirements in healthcare AI.

**Future Scope:**
Extend detection pipeline to full automated TIL scoring,
Segment tumor and stroma regions in histopathology slides,
Perform whole-slide image inference using multi-scale detection,
Improve performance using advanced augmentation and hyperparameter tuning,
Integrate explainable AI techniques for clinical trust,
Validate models with medical experts for real-world deployment.
