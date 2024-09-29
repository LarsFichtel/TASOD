# TASOD: A Data Collection for Tiny and Small Object Detection

## Introduction

This repository contains the dataset and code used in the paper **"TASOD: A Data Collection for Tiny and Small Object Detection"** presented at the ECCV 2024 AIM Workshop. The paper introduces TASOD, a novel dataset specifically designed to address the challenges of detecting tiny and small objects in images. The dataset includes 12,181 images and 207,745 annotated objects, providing a valuable resource for advancing object detection methods.

## Repository Structure

- `data/`: Contains the TASOD dataset.
  - `train/`: Training images and annotations.
  - `val/`: Validation images and annotations.
  - `test/`: Test images and annotations.
- `code/`: Source code for training and evaluating object detection models on TASOD.
  - `models/`: Implementations of various state-of-the-art object detection models.
  - `scripts/`: Scripts for data processing, training, and evaluation.
- `results/`: Benchmark results and qualitative analyses.
- `docs/`: Documentation and supplementary material related to the dataset and models.

## Dataset

### Overview

The TASOD dataset focuses on tiny and small object detection and is derived from existing datasets such as COCO, OpenImages, ImageNet, and more. Objects in TASOD are categorized into five size classes:
- **Tiny:** ≤ 8x8 pixels
- **Very Small:** > 8x8 pixels and ≤ 16x16 pixels
- **Small:** > 16x16 pixels and ≤ 32x32 pixels
- **Medium:** > 32x32 pixels and ≤ 96x96 pixels
- **Large:** > 96x96 pixels


## Getting Started

### Prerequisites

- Python 3.8+
- PyTorch
- MMDetection
- FiftyOne


## Results

Benchmark results for various models are provided in the results/ directory. The top-performing model in our experiments was Cascade R-CNN with a ResNeXt-101 backbone, achieving an AP50:5:95 of 25%.

## Qualitative Analysis

We conducted a qualitative analysis using the FiftyOne framework to inspect false positives and negatives. Insights from this analysis are also available in the results/ directory.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue if you have any suggestions or improvements.

## Acknowledgements

This research was supported by the Bavarian Academic Forum (BayWISS), the Center for Artificial Intelligence (CAIRO) from the Technical University of Applied Sciences Würzburg-Schweinfurt, and the Alexander von Humboldt Foundation.