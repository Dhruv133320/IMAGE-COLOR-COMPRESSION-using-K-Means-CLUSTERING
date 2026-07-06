# IMAGE-COLOR-COMPRESSION-using-K-Means-CLUSTERING
# 🎨 Image Color Compression using K-Means Clustering

A machine learning project demonstrating **image color compression** using the **K-Means Clustering** algorithm. Every pixel of an image is treated as a point in 3-dimensional RGB space, where K-Means groups similar colors into *k* clusters to reduce the total number of colors while preserving the overall visual quality.

---

# Problem Statement

Digital images often contain tens of thousands of unique colors, many of which are visually similar. Storing every unique color increases image complexity and storage requirements.

The objective of this project is to reduce the number of colors in an image using **K-Means Clustering**, creating a compressed version that remains visually similar to the original while requiring fewer representative colors.

---

# Dataset

Two sample images were used:

- 🦋 Butterfly
- 🦉 Barn Owl

Both images were analyzed and compressed using different values of **k**.

---

# Project Workflow

## 1. Data Preprocessing

- Load images using OpenCV
- Convert BGR images to RGB
- Reshape images into pixel matrices
- Count unique colors
- Visualize RGB distributions

---

## 2. Exploratory Data Analysis (EDA)

- Display original images
- Analyze image dimensions
- Calculate number of unique colors
- Plot RGB histograms
- Visualize pixel distribution in RGB space

---

## 3. Model Building

- Apply K-Means clustering
- Train on sampled pixels
- Compress images using different values of **k**
- Reconstruct compressed images
- Compare image quality

---

# Evaluation Metrics

The compression quality was evaluated using:

- Mean Squared Error (MSE)
- Peak Signal-to-Noise Ratio (PSNR)

Lower MSE indicates lower reconstruction error.

Higher PSNR indicates better image quality.

---

# Technologies Used

- Python
- NumPy
- OpenCV
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

# Results

The project demonstrates that:

- Increasing **k** improves image quality.
- Smaller values of **k** provide greater compression but lose image detail.
- Larger values of **k** preserve more colors while reducing compression efficiency.
- K-Means effectively identifies representative colors for image reconstruction.

---

# Repository Structure

```
IMAGE-COLOR-COMPRESSION/

│── Data preprocessing.ipynb
│── Eda color compression.ipynb
│── Model building.ipynb
│── butterfly.jpeg
│── barnowl.jpeg
│── README.md
```

---

# Inspiration

This project was inspired by the following open-source project:

**Repository:** https://github.com/tkarim45/Beginner-Data-Science-Projects

Specifically:

```
Image Color Compression (K-Means)
```

While inspired by the original idea and workflow, this project was independently implemented using different images, custom code, modified notebooks, and without relying on the original utility functions.

---

# Future Improvements

- Compare K-Means with MiniBatch K-Means
- Experiment with different color spaces (HSV, LAB)
- Build a web application for image compression
- Evaluate compression on larger image datasets

---

## Author

**Dhruv Borija**

GitHub: https://github.com/Dhruv133320
