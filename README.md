# AI-Assisted Image Analysis

This project is a rapid proof-of-concept exploring how quickly a working **computer vision (CV)** pipeline can be developed using AI-assisted coding. The goal was to simulate pathology-style object segmentation using synthetic asteroid images — enabling controlled, explainable analysis without sensitive or proprietary datasets.

---

## 📌 What Is Computer Vision?

**Computer Vision (CV)** is the field of using algorithms to extract meaning from images. It includes tasks like:
- Detecting objects (e.g., cells, tumors, asteroids)
- Measuring shape, size, and count
- Filtering noise, adjusting contrast, and enhancing visibility

In this project, we walk through a foundational CV pipeline using classic image processing techniques — not machine learning — to make the logic fully transparent.

---

## 🔍 Project Goals

- Show that AI-assisted development can produce working CV pipelines quickly
- Demonstrate real-world challenges in image processing: thresholding, contour fragmentation, object overlap, and noise
- Build a visually intuitive example that can be generalized to pathology, microscopy, or space imagery

---

## 🧠 Key Features

- Adaptive thresholding and Gaussian blur preprocessing
- Contour detection and area-based filtering
- Circularity filtering to exclude non-target shapes (e.g., elongated ships)
- Area histogram to guide `min_area` tuning
- Visual overlay of detected contours and object counts
- Contrast tuning using CLAHE (optional)

---

## 🌌 Why Asteroids?

This project simulates pathology-style object detection using **asteroid fields** instead of biological slides. This approach provides several key benefits:

1. **Visual clarity and storytelling**  
   Asteroids mimic the detection challenges in pathology — irregular shapes, overlap, noise — but are easier to reason about and far more engaging visually.

2. **No IP or data sensitivity issues**  
   All imagery was AI-generated, so there are no privacy or data ownership concerns. This makes the pipeline fully shareable and safe for public experimentation.

3. **Immediate transferability**  
   The exact pipeline logic — thresholding, contour filtering, shape metrics — applies directly to pathology, satellite imaging, or microscopy.

> This isn't a shortcut — it's a clean abstraction of the same core challenges you'd face in biomedical CV tasks.

---

## 🤖 AI-Assisted Development

This pipeline was built from scratch using **ChatGPT** as a coding assistant. Every step — from image generation to OpenCV filtering logic — was written collaboratively, then reviewed and debugged with full human oversight.

> AI made development faster — but human logic and QC made it correct.

---

## 📦 What's Included

- `Mining_Asteroids.ipynb` – Full annotated Jupyter notebook
- `*.png` images – AI-generated asteroid fields (with and without spaceships)
- `labeled_*.png` – Output images with visual overlays
- Inline visualization of thresholds, contours, and histograms
- Reusable pipeline for object detection on arbitrary grayscale images

---

## 🧪 Requirements

- Python 3.8+
- OpenCV (`opencv-python-headless` recommended for notebooks)
- NumPy
- Matplotlib

You can install everything with:

```bash
pip install opencv-python-headless numpy matplotlib





