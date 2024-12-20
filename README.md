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

## Acknowledgements
We would like to acknowledge the following works,

https://github.com/Sunojlab/Transfer_Learning_in_Catalysis

https://github.com/skinnider/low-data-generative-models

https://github.com/isayev/ReLeaSE

https://github.com/alhqlearn/REEXPLORE.git


