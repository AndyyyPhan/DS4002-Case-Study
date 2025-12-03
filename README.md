# DS4002 Fruit Freshness Classification Case Study

## Summary
This repository contains all materials for the **Fruit Freshness Classification Case Study**, where students build a deep learning model using transfer learning (ResNet-50) to classify fruit images by freshness.

The repository is organized as follows:

- **LICENSE.md** – License and citation information for this repository.  
- **SCRIPTS/** – All Python scripts and Jupyter notebooks used for dataset preparation, preprocessing, train/validation/test splitting, ResNet-50 model training, and evaluation.  
- **DATA/** – Raw fruit images and any cleaned, resized, or augmented datasets used during preprocessing.  
- **OUTPUT/** – All figures, metrics, and visual artifacts generated from training and evaluating the model.  
- **RUBRIC.pdf** – The grading rubric describing expectations for completing the case study.  
- **HOOK_DOCUMENT.pdf** – One-page introductory document that sets the scenario and motivates the project.  
- **SUPPLEMENTAL/** – Contains a blog-style explainer on transfer learning and a technical article supporting the methodology.

This repository provides all the resources needed to reproduce the fruit freshness classification pipeline and complete the case study.

---

## Reproducing Results

### **1. `01_train_val_test_split.py`**
Reads in the raw fruit dataset, validates folder structure, and generates stratified train/validation/test splits.  
**Output:**
- Organized directory structure under `DATA/dataset_splits/`
- Train/validation/test summary printed to console

---

### **2. `02_train_resnet50_colab.ipynb`**
Loads the processed dataset, applies preprocessing (resizing, normalization, augmentation), freezes the ResNet-50 base, attaches a custom classification head, and trains the model.  
**Output:**
- `classification_report.json`  
- `best_model.h5`  
- `training_history.json`  
- `confusion_matrix.png`

---

## References

[1] Bijoy, Md Hasan Imam; Tasnim, Syeda Zarin; Awsaf, Syed Ali; Hasan, Md Zahid (2025), “FruitVision: A Benchmark Dataset for Fresh, Rotten, and Formalin-mixed Fruit Detection”, Mendeley Data, V2, doi: 10.17632/xkbjx8959c.2  
[2] Shin, L. (2023). Chapter 3 — Transfer Learning with ResNet50: From Dataloaders to Training (Seed of Thought). Medium. https://medium.com/@lucrece.shin/chapter-3-transfer-learning-with-resnet50-from-dataloaders-to-training-seed-of-thought-67aaf83155bc  
[3] Paralect Team. (2022). Transfer Learning Applied. Paralect Blog. https://www.paralect.com/blog/post/transfer-learning-applied

