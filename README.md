# Face Recognition using PCA (Eigenfaces)

## Project Overview

This project implements a face recognition system using Principal Component Analysis (PCA) and the Eigenfaces approach.

The model is trained on the AT&T (ORL) Face Dataset and uses dimensionality reduction to represent facial images in a lower-dimensional eigenspace for efficient recognition.

This project was completed as part of the Machine Learning Summer of Code (SOC) mid-term project.

---

## Objectives

* Understand Principal Component Analysis (PCA)
* Learn dimensionality reduction techniques
* Implement Eigenfaces for face recognition
* Perform recognition on known and unknown faces
* Visualize eigenfaces and mean face representations

---

## Dataset

AT&T (ORL) Face Dataset

* 40 subjects
* 10 images per subject
* Grayscale facial images

---

## Methodology

1. Load and preprocess face images.
2. Flatten images into feature vectors.
3. Apply PCA for dimensionality reduction.
4. Generate Eigenfaces from principal components.
5. Project training images into eigenspace.
6. Compare query images using Euclidean distance.
7. Identify the closest matching face.

---

## Results

Training Matrix Shape:

```python
(389, 10304)
```

Top Explained Variance Ratios:

```python
[0.1778, 0.1290, 0.0667, 0.0563, 0.0513]
```

### Test A: Known Person

Query Image: s39/10.pgm

Prediction:

```python
s39
```

### Test B: Unknown Person

Query Image: s40/1.pgm

Closest Match:

```python
s5
```

---

## Libraries Used

* NumPy
* OpenCV
* Matplotlib
* Scikit-learn

---

## Repository Contents

* Face_Recognition_PCA.ipynb
* midterm_progress.md
* requirements.txt

---
