# Fruit Quality Detection

## Overview
This project implements a combined deep learning pipeline for fruit instance segmentation and quality classification.  
Using YOLOv8 for segmentation and a custom CNN for classification, it detects fruits and classifies their freshness status (fresh or rotten) across multiple fruit types.  
The segmentation model is trained on the FruitSeg30 dataset, while the classification model uses a small subset of a public fresh-rotten fruit dataset.

## Dataset Sources
- **Classification dataset:**  
  Fruits Fresh and Rotten Classification  
  [https://github.com/Bangkit-JKT2-D/fruits-fresh-rotten-classification](https://github.com/Bangkit-JKT2-D/fruits-fresh-rotten-classification/tree/master)

- **Segmentation dataset:**  
  Fruit Instance Segmentation Dataset (FruitSeg30)  
  [https://data.mendeley.com/datasets/vkht8pfsp3/3](https://data.mendeley.com/datasets/vkht8pfsp3/3)

## Important Notes
- Any reference or use of this project **must credit the author (@Rubick666)**.
- Due to hardware and internet limitations, the classification model was trained on a very small subset (~20 images per class).  
  For better performance, training on larger datasets is highly recommended.
- Segmentation model achieved a fitness score of ~0.96 with mAP50 around 0.52.
- Classification model achieved an overall accuracy of ~62% on the validation set, with detailed per-class metrics provided.

## Project Structure
├── classification/ # CNN classification model code and training scripts
├── FruitSeg30/ # YOLOv8 segmentation model code and training scripts
├── Dataset/ # Dataset preparation scripts and sample data
├── README.md # This documentation file
├── YOLO+CNN_to_detect_and_classifiy_fruits.ipynb

## Installation & Usage
1. Clone the repository:
git clone https://github.com/YourGitHubUsername/Fruit-Quality-Detection.git
2. Install required packages:
3. Prepare datasets as described in the `Dataset/` folder.
4. Train or evaluate models using scripts in `classification/` and `FruitSeg30/`.
5. Use provided notebooks or scripts for inference and visualization.

## Results Summary
- **Segmentation:**  
- Fitness: 0.9607  
- mAP50: ~0.52  
- Precision (Bounding boxes): 0.99  
- Recall (Bounding boxes): 0.50

- **Classification:**  
- Accuracy: ~62%  
- Per-class F1-scores vary; some classes have lower performance due to limited data.

## Contact
For questions or collaboration, contact: AMIRFARHAD_AMIRI@yahoo.com

---

Thank you for your interest in this project!
