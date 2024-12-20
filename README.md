# CFR: Classification Followed by Regression

# EnsembleAC: Deep Learning for Ligand Generation and %ee Prediction

## Prerequisites
Ensure you have the following installed before proceeding:
- **Python**: 3.7.16 (via Anaconda)
- **PyTorch**: 1.12.1
- **CUDA**: 11.3

## Environmental Setup
1. Create a new Conda environment:
   ```bash
   conda create --name EnsembleAC python=3.7.16
   conda activate EnsembleAC
   conda install pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.3 -c pytorch
   pip install -r requirements.txt

## Git Repositories
2. Clone these required repositories after setting up the environment:
   ```bash
   git clone https://github.com/fastai/fastai1.git

## Preparation
All datasets used for pre-training can be accessed via the link below:
https://drive.google.com/drive/folders/1bVTGxsm43jYrCcbuV5p2dxGYfbr5ZKYl?usp=drive_link

Please download the datasets and place them in the ./Data/Pretraining-data folder.

## Project Notebooks Overview
This repository contains a series of Jupyter notebooks for building CFR based models, and performing %Yield predictions.
# Project Overview

This repository contains several Jupyter notebooks for analyzing and predicting chemical reaction performance, including classification and regression tasks. Below is a description of each notebook:

## Notebooks Overview

1. **CFR-major_regression_code.ipynb**  
   This notebook implements regression models for the major class in the CFR (Classification Followed by Regression) approach, predicting key properties for the primary dataset.

2. **CFR-minor-regression-code.ipynb**  
   Focused on regression for the minor class in the CFR approach, this notebook handles less frequent reaction data and ensures balanced performance.

3. **DNN-classification.ipynb**  
   Implements a Deep Neural Network (DNN) for classifying the dataset into major and minor classes, based on reaction performance and features.

4. **DR vs CFR-plot.ipynb**  
   Generates comparative plots to analyze the performance difference between the Direct Regression (DR) and Classification Followed by Regression (CFR) methods.

5. **Yield distribution.ipynb**  
   Visualizes the distribution of yields in the dataset, providing insights into data skewness and class boundaries.

6. **classification_spider_plot.ipynb**  
   Creates spider plots to visualize the classification performance metrics, highlighting differences between major and minor classes.

7. **direct_regression_code.ipynb**  
   Implements the Direct Regression (DR) method, predicting properties without classifying the dataset beforehand.

8. **extract-ulmfitencoding-features.ipynb**  
   Extracts features using ULMFiT (Universal Language Model Fine-tuning) encoding for downstream tasks like classification and regression.

9. **heatmap_analysis.ipynb**  
   Generates heatmaps to analyze correlations and dependencies between various features and reaction outcomes.

10. **m-cha-performance-barplot.ipynb**  
    Creates bar plots to compare model performances on the meta-C-H activation (MCHA) dataset.

11. **pretrained_model_general_domain_LM.ipynb**  
    Demonstrates the use of a pre-trained general-domain language model for encoding and analyzing reaction data.

12. **smote.ipynb**  
    Applies the SMOTE (Synthetic Minority Oversampling Technique) method to address class imbalance in the dataset.

13. **tmap-plot.ipynb**  
    Visualizes reaction data using tMAP (Tree-Map) plots to identify patterns and clusters.

---

## Requirements
Refer to the [requirements.txt](./requirements.txt) file for details on dependencies.

## Notes
- These notebooks are designed for chemical reaction performance prediction tasks and are optimized for datasets with imbalanced classes.
- For detailed usage, check comments within each notebook or reach out to contributors.



## Acknowledgements
We would like to acknowledge the following works,

https://github.com/Sunojlab/Transfer_Learning_in_Catalysis

https://github.com/skinnider/low-data-generative-models

https://github.com/isayev/ReLeaSE

https://github.com/alhqlearn/REEXPLORE.git


