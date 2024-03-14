# HMS - Harmful Brain Activity Classification Kaggle Competition

## Overview
In the HMS - Harmful Brain Activity Classification Kaggle competition, our goal was to automate the classification of electroencephalography (EEG) and spectrogram data to detect harmful brain activity. The challenge was to enhance the accuracy and consistency of EEG pattern classification amidst diverse expert opinions. 

## Dataset
The dataset comprised EEG data and spectrogram images annotated by experts, with labels indicating various brain activity patterns. The key challenge was the data's noise, variability, and inconsistencies in expert annotations, along with significant label imbalance.

## Methodology
Our methodology employed a dual-approach: leveraging CatBoost for its categorical data efficiency and an ensemble of deep learning models, including ResNet34d, EfficientNetB0, and EfficientNetB1, to capture a broad spectrum of patterns within the EEG data.

## Experiments and Modifications
A series of experiments aimed to refine the models:
- **CatBoost Starter Modifications:** Adjustments to handle label imbalance and missing values.
- **Inference Ensemble Modifications:** Optimization of vote thresholds and segmentation strategies across ensemble models.
- **EfficientNetB0 Specific Experiments:** Pre-testing ensemble-designed experiments on EfficientNetB0 to assess impact before extending to the full ensemble.

Each experiment aimed to address specific issues, such as data reliability and model robustness, often revealing complex dynamics between data processing techniques and model performance.

## Results
The modifications led to varying degrees of success, with some improving the models modestly and others offering valuable insights into data characteristics and model sensitivities.

## Repository Contents
This repository contains all notebooks related to our experiments, modifications, and the submission process for the competition:
- `E1_CatBoost_Other_Labels_Reduction.ipynb`
- `E2_CatBoost_Other_Labels_Reduction_Nan_Values_Handling.ipynb`
- `E3_CatBoost_Label_Correction.ipynb`
- `E4_CatBoost_Vote_Counts_Segmented_Models_Training.ipynb`
- `E4_CatBoost_Vote_Counts_Segmented_Models_Submission.ipynb`
- `E5_CatBoost_training_less_more10_0.8_consensus.ipynb`
- `E6_Ensemble_*_less_than_4_removed.ipynb` (Multiple notebooks for different ensemble models)
- `E7_Ensemble_*_Vote_Counts_Segmented_Models.ipynb` (Multiple notebooks for different ensemble models)
- `E8_EffNetB0_Vote_Counts_Segmented_Models_*.ipynb`
- `E9_Leaky_EfficientNetB0_submission.ipynb`
- `E9_Leaky_EfficientNetB0_training.ipynb`

Each notebook is named according to the specific experiment and model it pertains to.

## Authors
- Neus Vegas
- Andreas Pattichis
- Alberto Carpes
