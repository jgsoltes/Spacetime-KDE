Generates and analyzes data for the Statistical Topography of Spacetime.

Dependencies:
- Core: numpy, pandas, matplotlib, seaborn, scipy, sklearn
    - hdim_opt (depends on numpy, scipy); for QUASAR optimization, Lorentzian KDE, sensitivity analysis, zero-phase component analysis
- Optional (using spacetime_histories.csv): joblib, tqdm, gplearn

Notes:
- Notebook is self-contained. First cells are reserved for function definitions, followed by the execution cells.
    - Each cell is titled for clarity. The corresponding functions provide docstrings defining the inputs and outputs.
    - plot_resolution = 'high' saves high-res plots; 'low' for faster analysis

Misc:
- Optimization cell defaults to a lower 'n_points'/'popsize'/'maxiter' block for testing; can uncomment top hyperparameter block for full reproducibility.
- Symbolic regression cell may be un-commented to generate new approximations.
