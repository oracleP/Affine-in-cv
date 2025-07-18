# Affine-in-cv
An Affine Transformation is a linear mapping method that preserves points, straight lines, and planes. It includes operations like:

Rotation

Translation

Scaling

Shearing

It uses 3 points to compute a 2×3 matrix which transforms the image accordingly.
# 🔄 Affine Transformation in OpenCV

This project demonstrates how to apply **Affine Transformations** to images using Python and OpenCV. Affine Transformation is a type of linear mapping that preserves geometric properties such as **points, straight lines, and planes**.

---

## 🎯 Objective

To understand and apply **Affine Transformations** including translation, rotation, scaling, and shearing using OpenCV's built-in functions.

---

## 🧰 Techniques Covered

- Rotation
- Translation
- Scaling
- Shearing
- Matrix transformation using 3 points

---

## 📐 What is an Affine Transformation?

An **Affine Transformation** is a geometric transformation that:
- Preserves **collinearity** (points remain on a line)
- Preserves **ratios of distances** (midpoints remain midpoints)
- Applies **linear mapping** (combinations of rotation, scaling, shearing, and translation)

It computes a **2×3 transformation matrix** using three non-collinear points from the input and their corresponding points in the output.

---

## 🖼️ How It Works

1. Select 3 points from the original image.
2. Define their corresponding locations in the output image.
3. Use `cv2.getAffineTransform(src_pts, dst_pts)` to compute the 2×3 matrix.
4. Apply transformation using `cv2.warpAffine()`.

---

## 🧱 Dependencies

- Python 3.x
- OpenCV
- NumPy

Install using:

```bash
pip install opencv-python numpy
