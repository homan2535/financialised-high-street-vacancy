# Financialised Brand Collapse and High-Street Vacancy

This repository contains the code and reproducibility materials for my
CASA0004 dissertation.

## Notebooks

- `H1_H3.ipynb`: matched event-study, robustness checks and H3 comparison
- `H2.ipynb`: DBSCAN, quadrat analysis, Moran's I and spatial maps

## Data

The analysis uses an openLocal longitudinal business-rates panel. The parquet
is not stored on GitHub because it is approximately 618 MB. See
`data/README.md` for access and file-placement instructions.

The LAD boundary GeoJSON is stored in the `data` directory.

## Running the analysis

1. Download the parquet and place it in `data/`, or allow the notebook to
   download it from the authorised Google Drive link.
2. Install the packages listed in `requirements.txt`.
3. Run `H1_H3.ipynb`.
4. Run `H2.ipynb`.

## Expected headline results

- H1 DiD-style difference: +16.98 percentage points
- Treated properties: 2,270
- Matched controls: 6,810
- H2 clustered share at 400m: 77.4%
- Site-level Moran's I: 0.105
- H3 amplification: +3.61 percentage points
