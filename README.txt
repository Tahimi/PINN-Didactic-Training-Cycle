================================================================
README: Supplementary Materials
================================================================

Title:  Physics-Informed Neural Networks: A Didactic 
        Derivation of the Complete Training Cycle

Journal: SIAM Review (Education Section)

================================================================
CONTENTS OF THIS ARCHIVE
================================================================

1. PINN_Didactic_Notebook.ipynb
   Interactive Jupyter Notebook (Python 3 / PyTorch)
   - Part 1: Reproduces every manual calculation from 
     Sections 2-3 of the manuscript using PyTorch's 
     automatic differentiation engine.
   - Part 2: Executes the full PINN training pipeline 
     (15,000 epochs) and generates all publication figures.

2. pinn_trained_model.pt
   Trained model checkpoint (PyTorch state_dict).
   Contains the 22 optimized parameters of the 1-3-3-1 MLP.

3. pinn_results.json
   Evaluation metrics and predictions: MSE, relative L2 
   error, pointwise predictions at selected evaluation 
   points. All numerical values in Section 4 of the 
   manuscript are read directly from this file.

4. pinn_loss_history.npz
   Epoch-by-epoch training loss history (NumPy compressed 
   archive). Contains arrays for total loss, L_R, and 
   L_IC at every epoch. Used to generate the loss 
   convergence figure.

5. figures/
   Publication-quality figures in PDF format:
   - training_cycle.pdf
   - mlp_architecture.pdf
   - neuron_detail.pdf
   - loss_history.pdf
   - validation_plot.pdf

6. index.html
   Index file for the supplementary materials.

================================================================
REQUIREMENTS
================================================================

- Python >= 3.8
- PyTorch >= 1.10
- NumPy >= 1.20
- Matplotlib >= 3.4

To install all dependencies:
    pip install torch numpy matplotlib

================================================================
HOW TO RUN
================================================================

Option A: Jupyter Notebook (local)
    jupyter notebook PINN_Didactic_Notebook.ipynb

Option B: Google Colab (no installation required)
    Upload the notebook to Google Colab. All dependencies 
    are pre-installed in the Colab environment.

The notebook is fully self-contained. Running all cells 
sequentially will:
  (a) Reproduce every hand-calculated value from the text
  (b) Train the PINN from scratch (approximately 30 
      seconds on CPU)
  (c) Generate all figures and evaluation metrics

A fixed random seed ensures full reproducibility across 
platforms.

================================================================
CONTACT
================================================================

Abdeladhim Tahimi
abdeladhim.tahimi@ceca.ufal.br
Universidade Federal de Alagoas (UFAL), Brazil
================================================================
