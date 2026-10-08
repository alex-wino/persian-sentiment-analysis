# Experimental Protocol

## Problem

Binary sentiment classification of Persian user reviews from a food-ordering service.

The task is to classify each review as either Positive or Negative.

## Primary Metric

The primary evaluation metric is macro-F1.

Secondary metrics include:

- Accuracy
- Precision and recall for each class
- F1 score for each class
- Confusion matrix

## Data Split

The primary dataset is provided with predefined train, validation, and test splits.

These existing splits will be preserved rather than re-created.

The exact number of samples and class distribution in each split will be documented during EDA.

A fixed random seed of `42` will be used for later randomized procedures where applicable.

## Data Quality

The dataset provider reports that duplicate samples have already been removed.

This claim will be checked during EDA, including the possibility of duplicates across splits.

No additional broad data-removal rule will be introduced before EDA.

## Evaluation Rules

- The test set will be used only for the final evaluation of P1.
- Model and configuration selection will be based on the validation set.
- Each controlled experiment should change one major factor at a time.
- Every experiment will be recorded in `experiments/results.csv`.
- Any change to the protocol will be documented here with its date and rationale.

## Reproducibility

The project will use fixed seeds where randomness is involved and will record the software environment and experiment settings needed to reproduce the results.
