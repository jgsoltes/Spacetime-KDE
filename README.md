Generates and analyzes data for the statistical topography of spacetime.

Dependencies:
- NUMPY v2.3 OR LOWER (for KDE calculations via 'numba').
- Core: pandas, matplotlib, seaborn, scipy, sklearn, hdim_opt.
- Optional (if not re-generating data): joblib, tqdm, gplearn, os.

Datasets:
- spacetime_ensemble.csv: The core data ensemble of spacetime coordinates, used to build the KDE.
- fluctuation_probs.csv: The exotic fluctuation probabilities, used in the analysis.

Usage:
- Notebook is self-contained. First cells are reserved for function definitions, followed by the execution cells.
- plot_resolution = 'high' for high-res plots; 'low' for faster analysis.
- Fully executable via 'run all'.
- Optimization and symbolic regression cells are commented out, to avoid length re-runs. Uncomment these cells if desired.

- Each cell is titled for clarity:
    - Cell 1: Imports, constant definitions, parameter bounds.
    - Cell 2: Defining the analysis functions to analyze the topography.
    - Cell 3: Defining the main functions to build the statistical topography.
    - Cell 4: Evolutionary optimization.
        -  Uncomment to test with the 'testing' hyperparameters, or uncomment the 'actual' hyperparameters to replicate the full dataset.
    - Cell 5: Building and analyzing the kernel density estimate (KDE).
    - Cell 6: Core analysis of the spacetime ensemble and its KDE probabilities.
    - Cell 7: Calculates the topographic evolution of coordinates as they follow probability gradients.
    - Cell 8: Exotic probabilities (KDE resonance + stochastic fluctuations).
    - Cell 9: Symbolic regression execution.
        - Uncomment to generate new analytical approximations.
    - Cell 10: Testing the symbolic analytical approximation.
Additional:
    - Cells 11-13: 'Future works' of the manuscript.
        - Biases probabilities by injecting electromagnetic energy.
        - Estimates the resulting number of particles created by the big bang.
