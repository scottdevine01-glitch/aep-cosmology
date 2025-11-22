# AEP Cosmic Superfluid Theory - Code Repository

This repository contains the code and data for the paper:  
**"The Anti-Entropic Principle and the Two-Field Cosmic Superfluid: A Unified Theory from Primordial Coupling to Late-Time Dissipation"**

## Reproducing the Results

The central predictions of the paper can be reproduced in two steps:

1.  **Solve for AEP Parameters:**
    ```bash
    python src/aep_solver.py
    ```
    This solves the coherence scale system and outputs the zero-parameter values for `g, λ, γ, κ, v_χ, λ_χ` to `data/best_fit_parameters.txt`.

2.  **Run Cosmological Integration:**
    ```bash
    python scripts/run_h0_calculation.py   # Generates H0 = 73.63
    python scripts/run_s8_calculation.py   # Generates S8 = 0.758
    ```

## Requirements
*   Python 3.8+
*   NumPy, SciPy
*   Modified CLASS (included in `src/modified_class/`)

## License
[Choose an open-source license, e.g., MIT]
