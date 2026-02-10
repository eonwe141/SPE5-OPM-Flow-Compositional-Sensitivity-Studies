# Compositional Reservoir Simulation Sensitivity Studies: Grid, Permeability, and Well Configuration Analysis Using OPM Flow

**Author:** Athar Nisar Padder  
**Date:** February 2026  
**Simulator:** OPM Flow 2025.10  

> [!IMPORTANT]
> **Data Availability Notice:**  
> The full simulation result files (restart, summary, and debug files) for the Grid Refinement and Permeability Sensitivity studies exceed GitHub storage limits.  
> They are hosted on **Zenodo** and can be downloaded here:  
> **[DOI: 10.5281/zenodo.XXXXXXX](https://zenodo.org)** *(Replace with actual link after uploading)*

## Abstract

This repository contains data, and input decks for a comprehensive parametric sensitivity study of compositional gas injection in reservoir systems. Using the open-source OPM Flow simulator, this project investigates numerical stability, computational scaling, and operational envelopes for CO2-EOR conversion workflows. The analysis is divided into three integrated studies: (1) Grid Refinement, (2) Permeability Sensitivity, and (3) Multi-Well Configuration Optimization.


## Key Findings

### 1. Grid Refinement Analysis
*   **Stability:** The numerical stability boundary at 15,000 rb/day injection is grid-independent, failing on both coarse (147 cells) and refined (1,176 cells) models.
*   **Scaling:** Grid refinement (8x cell count) increased computational cost by 3.7x, demonstrating favorable sub-linear scaling for sparse linear solvers.
*   **Conclusion:** Coarse-grid screening is sufficient for identifying operational envelopes in feasibility phases.

### 2. Permeability Sensitivity Analysis
*   **Feasibility:** High-permeability systems (2X) achieved 79% lower Gas-Oil Ratio (GOR) compared to low-permeability systems (0.5X).
*   **Operational Limits:** Low-permeability reservoirs exhibited rate sensitivity, with performance degradation at 15,000 rb/day. High-permeability reservoirs maintained stable production across all rates.
*   **Screening:** Permeability >100 mD is recommended for standard injection strategies; lower permeability requires WAG or foam assistance.

### 3. Multi-Well Configuration Study
*   **Efficiency:** Modified well patterns (2, 4, and 5-well configurations) reduced simulation timesteps by 90% (263 to ~25) compared to the baseline 3-well case.
*   **Robustness:** All alternative well geometries converged successfully, validating OPM Flow's capability for complex well architecture modeling.

## Reproducibility

### Prerequisites
*   **OPM Flow:** Version 2025.10 or later
*   **Python:** 3.8+ (for analysis scripts)
*   **Python Libraries:** pandas, matplotlib, seaborn

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Citation

If you use this data or workflow in your research, please cite:

> Padder, A. N. (2026). Compositional Reservoir Simulation Sensitivity Studies: Grid, Permeability, and Well Configuration Analysis Using OPM Flow. GitHub Repository. https://github.com/eonwe141/SPE5-OPM-Flow-Compositional-Sensitivity-Studies.git
EOF






