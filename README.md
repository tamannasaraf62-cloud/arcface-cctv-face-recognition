# ArcFace Face Recognition for CCTV Forensic Analysis

An experimental face recognition module for a CCTV forensic analysis pipeline, focusing on face analysis, identity embeddings, and ArcFace-based model training.

## 📌 Project Overview

This repository contains Jupyter Notebooks developed for the face recognition component of a multi-vendor CCTV/DVR/NVR forensic analysis project.

The objective is to explore face detection, face representation, and identity matching techniques that can support the analysis of surveillance footage.

The work includes:

* InsightFace-based face analysis.
* ArcFace model training experiments.
* Face embedding generation.
* Model evaluation and export preparation.
* GPU-accelerated experimentation using Google Colab.

> **Project status:** Research and development / experimental implementation. Performance in real-world CCTV conditions requires further validation.

---

## 🎯 Objectives

1. Explore face recognition models suitable for CCTV analysis.
2. Generate meaningful face embeddings for identity matching.
3. Investigate ArcFace-based training and verification.
4. Prepare model artifacts for potential integration with a larger forensic analysis pipeline.
5. Evaluate the feasibility of GPU-based face recognition experiments.

---

## 📂 Repository Structure

```text
arcface-cctv-face-recognition/
│
├── README.md
├── .gitignore
│
├── ArcFace_CCTV_Face_Recognition_Training.ipynb
│
└── arcface.ipynb
```

---

## 🧠 Notebooks

### 1. ArcFace CCTV Face Recognition Training

**File:** `ArcFace_CCTV_Face_Recognition_Training.ipynb`

This notebook explores an ArcFace training pipeline, including:

* Dataset acquisition and preparation.
* Face detection and alignment.
* Dataset and dataloader setup.
* IResNet-style backbone and ArcFace margin head.
* Model training.
* Checkpointing and resume support.
* Verification evaluation using cosine similarity.
* ROC/AUC and threshold analysis.
* Training curves.
* Model export preparation.

### 2. InsightFace Face Analysis

**File:** `arcface.ipynb`

This notebook explores InsightFace-based face analysis and recognition experiments.

The notebook includes:

* GPU and CUDA environment checks.
* InsightFace installation and setup.
* ONNX Runtime provider configuration.
* Buffalo_L face analysis model initialization.
* Face analysis experiments.
* Embedding and recognition-related experimentation.

---

## 🛠️ Technologies Used

* Python
* PyTorch
* Torchvision
* InsightFace
* ONNX Runtime
* OpenCV
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook
* Google Colab
* CUDA / GPU acceleration (where available)

---

## ⚙️ Execution Environment

The notebooks are designed for experimentation in Google Colab.

### Recommended Setup

1. Open the notebook in Google Colab.
2. Select a suitable runtime.
3. Install the dependencies specified in the notebook.
4. Configure the required dataset or model resources.
5. Execute the notebook cells in sequence.
6. Review the generated evaluation results and exported artifacts.

> **Note:** Package versions, GPU availability, and downloaded model resources may affect execution results.

---

## 📊 Evaluation

The ArcFace training notebook includes verification-oriented evaluation components such as:

* Cosine similarity.
* ROC curve and AUC analysis.
* Threshold selection.
* Training and validation monitoring.

Evaluation results should be interpreted in relation to the dataset and experimental configuration. Results on a benchmark dataset do not establish performance on all CCTV environments.

---

## 🔐 Data Privacy and Security

This repository should not contain:

* API credentials or authentication tokens.
* Private CCTV footage.
* Personally identifiable surveillance data.
* Unauthorized biometric data.
* Unapproved trained model artifacts.

Any deployment involving face recognition should consider authorization, privacy, data protection, security, and applicable legal requirements.

---

## 🚧 Current Limitations

* The notebooks are experimental and may require environment-specific adjustments.
* Dataset characteristics may differ from real-world CCTV footage.
* Model performance requires validation on representative surveillance conditions.
* Face recognition accuracy can be affected by blur, lighting, occlusion, camera angle, and image quality.
* Integration with the complete forensic analysis pipeline is a separate engineering task.

---

## 🔮 Future Scope

* Evaluation on representative CCTV datasets.
* Robustness testing under low-light and occlusion conditions.
* Improved identity matching and threshold calibration.
* Integration with the project's forensic processing pipeline.
* Reproducible experiment configurations and model versioning.
* Security and privacy validation before any operational deployment.

---

## 👥 Project Context

This work is part of a broader CCTV/DVR/NVR forensic analysis project for surveillance evidence processing.

The face recognition component is intended to be developed as one part of the larger system, alongside other forensic analysis and evidence-handling capabilities.

---

## 📄 License

Add an appropriate license after confirming the team's project ownership and distribution requirements.
