# Advanced Computer Vision for AI - ARI3129

## Traffic Sign Detection and Attribute Classification

This project focuses on the detection of traffic signs and the classification of their attributes using object detector models.

## Project Structure

### Notebooks

- **[`1_data_visualisation.ipynb`](1_data_visualisation.ipynb)**: Initial exploration and visualisation of the dataset. Includes visualisation of the annotation distribution (individual and merged) and map of the dataset.

#### Attribute Classification (`notebooks_attributes/`)
The following notebooks explore attribute classification (Mounting Type, Sign Conditions, Viewing Angle, Shape) for the detected traffic signs:
- [`2b_MountingType_DanielGalea.ipynb`](notebooks_attributes/2b_MountingType_DanielGalea.ipynb)
- [`2b_SignConditions_LiamAzzopardi.ipynb`](notebooks_attributes/2b_SignConditions_LiamAzzopardi.ipynb)
- [`2b_ViewingAngle_MatthewPrivitera.ipynb`](notebooks_attributes/2b_ViewingAngle_MatthewPrivitera.ipynb)
- [`2b_sign_shape_LiamJakeVella.ipynb`](notebooks_attributes/2b_sign_shape_LiamJakeVella.ipynb)

#### Object Detection (`notebooks_detectors/`)
The following notebooks implement and evaluate different object detection architectures:
- [`2a_RF_DETR_MatthewPrivitera.ipynb`](notebooks_detectors/2a_RF_DETR_MatthewPrivitera.ipynb)
- [`2a_YOLOV11_DanielGalea.ipynb`](notebooks_detectors/2a_YOLOV11_DanielGalea.ipynb)
- [`2a_YOLOv12n_LiamJakeVella.ipynb`](notebooks_detectors/2a_YOLOv12n_LiamJakeVella.ipynb)
- [`2a_YOLOv8_LiamAzzopardi.ipynb`](notebooks_detectors/2a_YOLOv8_LiamAzzopardi.ipynb) 

### Results Comparison (`results_comparison/`)

The `results_comparison/` folder contains **[2c_results_comparison.ipynb](results_comparison/2c_results_comparison.ipynb)**. The notebook is divided into two parts: Sign Detector Analysis + Comparison and Sign Attributes Model Comparison/Analysis.
 
### Data Folder

The `data/` directory contains the dataset and annotations used throughout the project:

- **images/**: Contains the merged dataset of traffic sign images.
- **annotations/**:
  - **Individuals/**: Contains the individual JSON annotation files from each group member:
    - `input_Daniel_Simon_Galea.json`
    - `input_Liam_Azzopardi.json`
    - `input_Liam_Jake_Vella.json`
    - `input_Matthew_Privitera.json`
  - `COCO.json`: The final dataset annotations in COCO format.
  - `merged_input.json`: The combined annotation file from all team members.
  - **YOLO Labels/**: Annotations converted to YOLO format for training detector models.

### Environment & Dependencies

The project environment is defined in `Dependencies.yml` (the same one that was given in the group project resources).

### Trained Models

Due to file size restrictions, the trained models have been uploaded to [Google Drive](https://drive.google.com/drive/folders/1KNj_uAgLaKCxyCTztxPnd9kfeX1saIVE?usp=sharing).