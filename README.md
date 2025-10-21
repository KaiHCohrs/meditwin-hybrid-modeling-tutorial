# MeDiTwin Hybrid Modeling Tutorial

This repository contains materials for a hybrid modeling tutorial as part of the MeDiTwin Intelligent Earth Training funded by the European Union's Horizon Europe research and innovation program. The tutorial demonstrates advanced machine learning techniques for combining physics-based knowledge with data-driven approaches.

## Tutorial Overview

The tutorial consists of the demonstration of two flavors of hybrid modeling for estimating physical parameters:

### Part 1: Physics-Informed Neural Networks for Inverse Modeling
**File:** `Part_1_Physics_Informed_Neural_Networks_for_Inverse_Modeling.ipynb`

- **Focus:** Parameter estimation using Physics-Informed Neural Networks (PINNs)
- **Problem:** Estimate unknown mass parameter `m` in a damped harmonic oscillator from limited data
- **Key Learning:** How to combine data fitting with physics constraints to infer unknown parameters

### Part 2: Semi-parametric Hybrid Modeling
**File:** `Part_2_Semi_parametric_Hybrid_Modeling.ipynb`

- **Focus:** Q10 parameter estimation in ecosystem respiration modeling
- **Problem:** Estimate temperature sensitivity parameter Q10 from environmental data
- **Key Learning:** Understand and explore challenges of the semi-parametric hybrid modeling approach.

## Dataset

**File:** Synthetic `data/respiration.csv`

- **Features:** 
  - `x0`: Air temperature (T_A)
  - `x1`, `x2`, `x3`: Additional environmental covariates
  - `y`: True respiration values
  - `y_obs`: Observed (noisy) respiration values
  - `scenario`: Train/test split indicator
- **Split:** 505 training samples, 505 test samples

## Getting Started

### Prerequisites
- Google Colab (recommended) or Jupyter environment
- Python packages: `torch`, `torchvision`, `matplotlib`, `numpy`, `pandas`

### Installation
The notebooks include automatic package installation cells. Simply run the first cell in each notebook to install dependencies.

### Running the Tutorial
1. **Part 1:** Open `Part_1_Physics_Informed_Neural_Networks_for_Inverse_Modeling.ipynb`
   - Complete the TODO sections for physics loss computation
   - Observe how the PINN learns the unknown mass parameter
   
2. **Part 2:** Open `Part_2_Semi_parametric_Hybrid_Modeling.ipynb`
   - Experiment with different model configurations
   - Compare Q10 estimates across different settings
   - Submit your final Q10 estimate


## 🤝 Contributing

This tutorial is part of the MeDiTwin Intelligent Earth Training funded by the European Union's Horizon Europe research and innovation program under Grant Agreement No 101159723. For questions or issues, please contact the instructor.

## 📄 License

This material is provided for educational purposes as part of the MeDiTwin project.

---

**Note:** These notebooks are designed to run in Google Colab with no additional setup required. Simply open the notebooks and run the cells in sequence.
