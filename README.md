# Automatic Labeling of Coronary Artery Segments: Multi-Strategy Development and Evaluation

## Overview

This repository contains the complete implementation of the methods and experiments developed for the bachelor’s thesis **“Automatic Labeling of Coronary Artery Segments: Multi-Strategy Development and Evaluation.”** The project was conducted by Maren Clapers Colet (UPF), under the supervision of Pr. Oscar Camara Rey and César Acebes Pinilla, in collaboration with the engineering team at the Dimension Lab of Hospital de la Santa Creu i Sant Pau.

The aim of the project is to advance the automatic labeling of standard coronary artery segments from 3D segmentations, following the American Heart Association (AHA) scheme, to support and streamline the clinical workflow for the diagnosis of coronary artery disease (CAD).

## Project Objectives

- Develop, implement, and compare a variety of computational strategies for the automatic labeling of coronary artery segments.
- Integrate clinical knowledge, topological analysis, and artificial intelligence approaches (including heuristic, machine learning, and deep learning methods).
- Create a clinically validated ground truth dataset, based on the ASOCA public dataset.
- Evaluate the strengths, limitations, and clinical applicability of each method, and contribute practical tools to the AI-assisted cardiac diagnosis workflow.

## Methods

The repository includes the following main methods and pipelines:

1. **Heuristic-Based and Geometric Processing**
   - Curvature and bifurcation-based segmentation.
   - Heuristic and topological rules using graph representations and anatomical features (including heart chamber proximity).

2. **Machine Learning Approaches**
   - Classical ML using only centerline coordinates.
   - ML using graph-derived features (Minimum Spanning Tree and local topology).
   - Segment transition detection as a classification problem.

3. **Graph Neural Networks**
   - GraphSAGE for direct segment classification on coronary tree graphs.

4. **Direct Multi-class Segmentation**
   - Multi-class 3D segmentation with nnU-Net for end-to-end coronary segment labeling from CCTA images.

## Dataset

- **Base Data:** The ASOCA dataset (Automated Segmentation of Coronary Arteries), containing 3D CCTA images and arterial segmentations.
- **Ground Truth:** Manual annotation and re-labeling of segments following the 18-segment AHA/SCCT standard, validated by clinical experts.
- **Preprocessing:** Centerline extraction, skeletonization, separation into RCA and LCA, and conversion to graph representations.

> **Note:** Raw medical images and manual annotations are not distributed in this repository.
