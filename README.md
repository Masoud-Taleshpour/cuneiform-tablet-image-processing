# Cuneiform Character Detection using Classical Computer Vision

## 📌 Project Overview
This project is part of my M.Sc. thesis. The goal is to detect and extract cuneiform wedges from images of ancient clay tablets.

## 🧠 Why Classical Computer Vision?
In this project, we operated under a strict assumption: **Extreme Data Scarcity**. 
We only had a small set of images (about 12 tablets) and **no labeled Ground Truth** (no bounding boxes or segmentation masks). Therefore, training Deep Learning models (like YOLO or Mask R-CNN) was impossible. I designed a classical image processing pipeline to extract features mathematically.

<img width="554" height="291" alt="image" src="https://github.com/user-attachments/assets/4a45551f-3744-4c07-b395-7e2b06e900e5" />

## ⚙️ Methodology
1. **Pre-processing:** Illumination correction and noise reduction.
2. **Morphological Filtering:** Identifying potential core regions.
3. **Region Growing:** Expanding seeds to capture the full wedge shape.
4. **Geometric Analysis:** Calculating orientation and bounding areas.


## ⚠️ Limitations & Future Work
Because this is a heuristic approach, parameters (like brightness thresholds) are manually calibrated for specific image resolutions. In the future, creating a labeled dataset to train adaptive or Deep Learning models would make the pipeline robust against varying lighting and tablet conditions.
