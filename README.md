# MEARN: Enhancing B-cell Epitope Prediction with ESM-Derived Protein Embeddings and Attention-Residual Neural Network
## Overview
This repository provides the implementation of MEARN, an Attention–Residual neural network for linear B-cell epitope prediction using protein embeddings extracted from the ESM-2 protein language model.  
All experimental results reported in the manuscript can be reproduced using the provided scripts and trained model.  
The final trained model weights are provided in HDF5 (.h5) format, while the complete network architecture and evaluation pipeline are fully defined in the source code.
## Requirements
- Python ≥ 3.8
- PyTorch ≥ 1.12
- CUDA-enabled GPU (recommended)
- fair-esm (ESM-2 pretrained model, checkpoint: esm2_t33_650M_UR50D)
- scikit-learn
- numpy
- pandas
- tqdm
- h5py
## File Description
- `extract_esm2_Mean-pool.py`  
  Extracts sequence-level ESM-2 embeddings using mean pooling.
- `extract_esm2_residue.py`  
  Extracts residue-level ESM-2 embeddings.
- `built_model.py`  
  Trains the MEARN model on the full training dataset and saves the final trained model.
- `cross_validation.py`  
  Performs k-fold cross-validation on the training set.
- `test_independent.py`  
  Trains the model on the full training set and evaluates it on the independent test set.
- `main.py`  
  Pipeline controller for training, cross-validation, and independent testing.
## Running the Pipeline
  Step 1. Extract ESM-2 embeddings from protein sequences (mean-pooled or residue-level).
  Step 2. Train the MEARN model on the training set.
  Step 3. Perform cross-validation to assess model robustness (optional).
  Step 4. Retrain the model on the full training set and evaluate on the independent test set.   
