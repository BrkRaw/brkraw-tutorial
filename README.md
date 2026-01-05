# BrkRaw Tutorial (Jupyter Notebooks)

This repository contains English tutorials for the updated BrkRaw API using the
example datasets hosted via Git LFS.

## Notebooks

- `notebooks/00_getting_started.ipynb` — install, download example data, and run
  core BrkRaw workflows (info, metadata, conversion).
- `notebooks/01_orientation_unwrap_vs_pose.ipynb` — compare unwrap pose vs
  subject pose, reorient to RAS, and visualize the differences.

## Launch on Binder

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/BrkRaw/brkraw-tutorial/HEAD?labpath=notebooks/00_getting_started.ipynb)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/BrkRaw/brkraw-tutorial/HEAD?labpath=notebooks/01_orientation_unwrap_vs_pose.ipynb)

## Local setup (recommended for Git LFS)

```bash
git lfs install

git clone https://github.com/BrkRaw/brkraw-dataset

# Create the tutorial environment
conda env create -f environment.yml
conda activate brkraw-tutorial

jupyter lab
```

## Notes

- The example datasets are stored in the `brkraw-dataset` repo using Git LFS.
  Make sure Git LFS is installed before cloning so you get the actual data.
- The notebooks assume the dataset repo lives at `data/brkraw-dataset`.
