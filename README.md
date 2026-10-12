# SHL Grammar Scoring Engine

## Project Overview
This project predicts continuous grammar scores from spoken-audio recordings using engineered acoustic features and machine learning.

## Objective
Predict grammar scores on a scale from 0 to 5 using audio-derived numerical features.

## Dataset
The competition dataset contains labelled training recordings and a separate test set. The audio files and original dataset are not included in this repository.

## Approach
- Extracted acoustic, temporal, and prosodic features from speech recordings.
- Applied data cleaning to handle missing and non-finite feature values.
- Evaluated regression models using cross-validation.
- Selected an Extra Trees Regressor based on validation performance.
- Generated continuous predictions within the valid score range of 0 to 5.

## Evaluation
The best recorded Kaggle public leaderboard score for the submitted solution was **0.7366**.

The notebook also reports training RMSE, training Pearson correlation, and cross-validation RMSE. Training and validation metrics are reported separately because training performance does not represent generalization to unseen data.

## Repository Contents
- `shl-grammar-scoring-experiment-02-advanced-fea.ipynb`: Experiment notebook.
- `submission_60features (1) (1).csv`: Submitted prediction file.
- `LICENSE`: MIT License.

## Reproducibility
The notebook documents the experimental workflow and evaluation. Access to the original competition dataset is required to rerun the feature extraction and training process.

## License
This project is released under the MIT License, subject to the competition's rules and restrictions on the underlying dataset.
