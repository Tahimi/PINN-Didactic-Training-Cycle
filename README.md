# PINN Complete Training Cycle

Companion code for:

**"Physics-Informed Neural Networks: A Didactic Derivation 
of the Complete Training Cycle"**

by Abdeladhim Tahimi  
Campus de Engenharias e Ciências Agrárias (CECA), 
Universidade Federal de Alagoas (UFAL), Brazil

## Contents

- `PINN_Didactic_Notebook.ipynb` — Interactive 
  Jupyter/PyTorch notebook that:
  1. Reproduces every manual calculation from the paper 
     using PyTorch's automatic differentiation engine
  2. Executes the full PINN training and validation 
     pipeline
  3. Generates all publication figures

## Computational Artifacts

- `pinn_trained_model.pt` — Trained model checkpoint
- `pinn_results.json` — Evaluation metrics and predictions
- `pinn_loss_history.npz` — Epoch-by-epoch loss history

## Requirements

- Python 3.8+
- PyTorch 2.0+
- NumPy
- Matplotlib

## Usage

Open the notebook in Jupyter or Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Tahimi/PINN-Didactic-Training-Cycle/blob/main/PINN_Didactic_Notebook.ipynb)

## Citation

If you use this code, please cite:

```bibtex
@article{tahimi2026pinn,
  author  = {A. Tahimi},
  title   = {Physics-Informed Neural Networks: A Didactic 
             Derivation of the Complete Training Cycle},
  journal = {Submitted to SIAM Review},
  year    = {2026},
}
