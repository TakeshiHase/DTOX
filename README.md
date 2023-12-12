# A Deep neural network-based in visio lens for large scale Toxicogenomics data
## Introduction
This repository contains the deep neural network-based models for 3D-surface images in Percellome database and scripts to run analysis pipeline based on the models to predict classes of the images and to perform explainability analysis, described in out paper, "DTox: A Deep neural network-based in visio lens for large scale Toxicogenomics data". 
## Citation
If you use the model and scripts for your study, please cite our article: Takeshi Hase, Samik Ghosh,  Ken-ichi Aisaki, Satoshi Kitajima, Jun Kanno, Hiroaki Kitano, and Ayako Yachie, DTox: A Deep neural network-based in visio lens for large scale Toxicogenomics data, The Journal of Toxicological Sciences, (in Press)
## Setup
We run the scripts (Jupyter notebooks) on Python3.11.3 with the following packages;
torch==2.1.0
torchvision==0.16.0
torchcam==0.4.0
## How to use
Open and run jupyter notebooks, prediction.ipynb and explainability_analysis.ipynb, to predict of classes of 3D-surface images and to perform explainability analysis, respectively. 
prediction.ipynb loads optimized deep convoluational neural network model for angle 1 ('resnet18.pth') and predicts classes for sample 3D-surface images in a directory for the samples ('./sample_data/'). 'prediction_results.txt' includes prediction results for each 3D-surface images. 
explainability_analysis.ipynb loads optimized deep convoluational neural network model for explainability analysis ('model_for_Xgrad.pth') for angle 1 and performs explainability analysis for sample 3D-surface images in a directory for the samples ('./sample_data/') based on Xgrad algorithm.
