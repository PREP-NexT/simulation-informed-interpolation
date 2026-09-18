# Simulation-informed rainfall interpolation

This repository contains research code supporting a manuscript on monthly rainfall interpolation in Singapore. The method uses climate-model simulations to define a Gaussian-process prior, calibrates station-specific noise from observations, and applies ordinary kriging to the remaining spatial residuals.

## Current status

The manuscript is under revision and this repository is still being organized. This README is a temporary overview; a publication-ready release will add a clean environment specification, data provenance, an end-to-end reproduction workflow, and detailed documentation.

## Main contents

- `utils.py`: core Gaussian-process interpolation and evaluation functions.
- `two_stage_validation.ipynb`: leave-one-station-out validation of the two-stage method.
- `kge_three_row_composite.ipynb`: consolidated KGE comparison and diagnostic figure.
- `sn_initialization_sweep.ipynb`: station-noise initialization sensitivity experiment.
- `gaussian_check.ipynb`: station–month rainfall distribution diagnostics.
- `data/`: observational and simulation inputs used by the notebooks.
- `figures/`: generated manuscript and revision figures.

## Use

Run the notebooks from the repository root. The current workflows use the standard Python scientific stack together with scikit-learn, PyKrige, GeoPandas, and Cartopy. Exact dependency versions and reproducibility instructions will be provided during the planned repository cleanup.

## Citation

Citation information will be added when the associated manuscript is published.
