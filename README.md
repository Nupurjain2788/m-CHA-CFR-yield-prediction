

# CFR (Classification followed by Regression) based model for yield prediction of m-CHA reaction dataset

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

## Dataset and Pretraining Weights

All datasets used for pre-training can be accessed via the link below:

(https://drive.google.com/drive/folders/1bVTGxsm43jYrCcbuV5p2dxGYfbr5ZKYl?usp=drive_link)

Please download the datasets and place them in the `./Data/Pretraining-dataset` folder.

### Pretraining Weights and Biases
Pretraining weights and biases can also be found in the provided Google Drive folder. After downloading, upload the weights into the `./Data/Pretraining_weights_bias` folder for proper model initialization.

# Project Overview

## Code

A) The notebook for pre-training the language model is given in the ‘Pre-training’ folder.

B) All the notebooks for regressor fine-tuning for DR and CFR methods are present in the ‘Fine-tuning’ folder.
- **direct_regression_code.ipynb**  
   Implements the Direct Regression (DR) method, predicting yield for the reaction dataset.
  
- **CFR-major_regression_code.ipynb**  
   This notebook implements regression models for the major class in the CFR (Classification Followed by Regression) approach, predicting yield for the reaction dataset.
   
 - **CFR-minor-regression-code.ipynb**  
   Focused on regression for the minor class in the CFR approach, predicting yield for the reaction dataset.
  
This repository contains several Jupyter notebooks for analyzing and predicting yield prediction for chemical reaction performance. Below is a description of each notebook:

## Notebooks Overview

- **DNN-classification.ipynb**  
   Implements a Deep Neural Network (DNN) for classifying the dataset into major and minor classes, based on ULMFiT model extracting encoding features.

 - **DR vs CFR-plot.ipynb**  
   Generates comparative plots to analyze the performance difference between the Direct Regression (DR) and Classification Followed by Regression (CFR) methods.

- **Yield distribution.ipynb**  
   Visualizes the distribution of yields in the dataset, providing insights into data skewness and class boundaries.

- **classification_spider_plot.ipynb**  
   Creates spider plots to visualize the classification performance metrics, highlighting differences between major and minor classes.

- **extract-ulmfitencoding-features.ipynb**  
   Extracts features using ULMFiT (Universal Language Model Fine-tuning) encoding for downstream tasks like classification and regression.

- **heatmap_analysis.ipynb**  
   Generates heatmaps to analyze correlations and dependencies between various reaction partners.

- **m-cha-performance-barplot.ipynb**  
    Creates bar plots to compare model performances on the m-CHA dataset.

- **pretrained_model_general_domain_LM.ipynb**  
    Demonstrates the use of a pre-trained general-domain language model for encoding and analyzing reaction data.

- **smote.ipynb**  
    Applies the SMOTE (Synthetic Minority Oversampling Technique) method to address class imbalance in the dataset.

- **tmap-plot.ipynb**  
    Visualizes reaction data using tMAP (Tree-Map) plots to identify patterns and clusters.

---

## Notes
- These notebooks are designed for chemical reaction performance prediction tasks and are optimized for datasets with imbalanced classes.
- For detailed usage, check comments within each notebook or reach out to contributors.



## Acknowledgements
We would like to acknowledge the following works,

https://github.com/Sunojlab/Transfer_Learning_in_Catalysis

https://github.com/skinnider/low-data-generative-models

https://github.com/isayev/ReLeaSE

https://github.com/alhqlearn/REEXPLORE.git


