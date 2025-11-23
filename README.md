# Investigating Knowledge Distillation of BERT Models

## Abstract
This project investigates **Attention-Based Knowledge Distillation (KD)** to compress a 12-layer BERT teacher into a 4-layer student model. We formulate a **non-stationary loss function** to project the teacher manifold onto a sparse student, minimizing **latent divergence** via attention-based regularization.

## Key Outcomes
- **Optimization:** Utilized a time-dependent exponential decay coefficient to balance supervised mimicry and autonomous learning.
- **Results:** Achieved **79% parameter reduction** (110M $\to$ 24M) with only an 11% tradeoff in accuracy on the GLUE SST-2 benchmark.
- **Methodology:** Addressed the "skip" and "search" layer misalignment problems using combinatorial optimization strategies.

## Files in this Repository
- `DL Final Report _1_.docx`: The full mathematical formulation and experimental results.
- `kd_pre_attn_results.ipynb`: The Jupyter Notebook containing the training pipeline, loss function implementation, and validation metrics.

## Usage
To replicate the distillation process:
1. Open `Model_Training.ipynb`.
2. Ensure dependencies (PyTorch, Transformers, TextAttack) are installed.
3. Run the training loop with the defined hyperparameters.

---
*Author: Ali Anser Jaffri*
