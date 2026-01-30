# Nano-Particle-Segmentation-from-TEM-images-with-Classical-Image-Processing
Classical image processing pipeline for nanoparticle segmentation in TEM images using Gaussian filtering, CLAHE, thresholding, morphology and watershed. Includes border removal, particle counting and evaluation using DICE, IoU and Hausdorff metrics.
TEM Nanoparticle Segmentation

#This project implements a classical image processing pipeline for segmenting nanoparticles in Transmission Electron Microscopy (TEM) images. The goal is to detect and analyse nanoparticle regions without using machine learning or deep learning models.

Pipeline Overview

The segmentation pipeline consists of:

Grayscale conversion

Gaussian smoothing for noise reduction

CLAHE for contrast enhancement

Otsu thresholding for foreground extraction

Morphological opening and closing

Watershed for splitting merged particles

Border removal of incomplete particles

Connected components for particle counting
Evaluation

Segmentation quality is evaluated using:

DICE coefficient

Intersection over Union (IoU)

Hausdorff distance

Particle counts are also compared with ground truth.

Results Summary

The classical pipeline achieves moderate segmentation performance. While most nanoparticle regions are detected, errors remain due to noise, overlapping particles, and ambiguous boundaries. This highlights the limitations of traditional image processing for complex microscopy data.
