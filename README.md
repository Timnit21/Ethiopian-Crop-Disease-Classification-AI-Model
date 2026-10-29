# Ethiopian-Crop-Disease-Classification-AI-Model
Open-source AI project for crop disease detection using leaf images, transfer learning, PlantVillage, and locally collected agricultural data.
# External Crop Disease Image Dataset

**Project:** AI-Based Crop Disease Classification  
**Organization:** Malam Engineering — Enterprise Application and AI  
**Dataset Type:** External Evaluation Dataset  
**Crops Covered:** Tomato, Potato, and Maize  
**Dataset Size:** 300+ images

## 1. Overview

This dataset contains more than 300 externally sourced images of tomato, potato, and maize plants. It was prepared to evaluate the performance and generalization capability of a trained crop disease classification model developed using the PlantVillage repository.

Unlike images drawn exclusively from PlantVillage, this dataset is intended to introduce variation in image backgrounds, lighting, leaf appearance, and environmental conditions. This helps assess whether the model can make reliable predictions on unfamiliar images.

## 2. Objectives

- Evaluate the model using images independent of its training dataset.
- Assess predictions across tomato, potato, and maize.
- Examine model robustness under different image and background conditions.
- Identify incorrect predictions and potential weaknesses.
- Measure classification performance using appropriate evaluation metrics.

## 3. Crop Categories

The dataset covers the following crops:

| Crop | Evaluation focus |
|---|---|
| Tomato | Healthy leaves and supported disease categories |
| Potato | Healthy leaves and supported disease categories |
| Maize | Healthy leaves and supported disease categories |

The specific disease classes and number of images per class should be documented based on the actual contents of the dataset.

## 4. Dataset Sources

Images are collected from external sources, such as publicly accessible online image collections and relevant agricultural resources, rather than intentionally copied from the PlantVillage training images.

The source, original URL, class label, and usage permissions should be recorded for each image wherever possible.

**Note:** External sourcing alone does not guarantee that an image is absent from the model's training data. Duplicate and near-duplicate images should be checked before final evaluation.

## 5. Recommended Directory Structure

```text
External_Crop_Disease_Test_Dataset/
├── README.md
├── tomato/
│   ├── healthy/
│   ├── early_blight/
│   └── other_disease_classes/
├── potato/
│   ├── healthy/
│   ├── early_blight/
│   └── other_disease_classes/
├── maize/
│   ├── healthy/
│   ├── common_rust/
│   └── other_disease_classes/
└── metadata/
    └── image_sources.csv
```

*This is a recommended structure. Adjust the folders to match the classes actually collected.*

## 6. Evaluation Methodology

The dataset is intended for independent model evaluation. The trained model should predict the appropriate class for each eligible
