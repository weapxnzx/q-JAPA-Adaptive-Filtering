# q-JAPA Adaptive Filtering

Implementation of the q-Jackson Affine Projection Algorithm (q-JAPA) for adaptive filtering under correlated inputs.

## Overview
This repository contains the reference implementation of the q-Jackson Affine Projection Algorithm (q-JAPA), a q-calculus-based extension of the classical Affine Projection Algorithm (APA). The proposed method incorporates the Jackson q-derivative into the adaptation process, introducing a data-dependent diagonal regularization mechanism that can improve convergence and tracking performance in correlated environments.

## Applications

- ECG artifact cancellation
- Convergence dynamics analysis

## Repository Structure

q_japa_algorithm.py
experiments/
├── exp1_ecg_artifact_cancellation.py
└── exp2_tracking_learning_curve.py

## Requirements

pip install -r requirements.txt

## Running the Experiments

### Experiment 1

Demonstrates the application of q-JAPA to adaptive noise cancellation using real ECG recordings from the MIT-BIH Arrhythmia Database.

python experiments/exp1_ecg_artifact_cancellation.py

### Experiment 2

Evaluates the tracking performance of q-JAPA under abrupt system changes and compares its learning behavior against the classical JAPA algorithm (q = 1).

python experiments/exp2_tracking_learning_curve.py

## Author

Jusset Zaid Soto Islas

## Citation

If you use this software in your research, please cite the associated publication and the Zenodo DOI.
