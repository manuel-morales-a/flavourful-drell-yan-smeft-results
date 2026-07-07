# PDF Uncertainties across Flavour Space in High-Energy Drell-Yan SMEFT Analyses

This repository will host machine-readable ancillary files for the numerical results associated with this paper.

Authors:

- David Marzocca
- Manuel Morales-Alvarado

Affiliation:

- INFN, Sezione di Trieste, Via Bonomea 265, 34136 Trieste, Italy

The numerical files will support the paper's study of high-mass Drell-Yan constraints on semileptonic SMEFT operators, comparing fixed and profiled parton-distribution treatments across quark-flavour scenarios and HL-LHC projections.

## Status

This repository skeleton is prepared for ancillary results. Numerical result files are not included yet.

Paper identifiers:

- arXiv: TBD
- DOI: TBD
- Journal reference: TBD

## Repository layout

```text
metadata/
  paper.yaml          Paper metadata and citation placeholders.
  conventions.md     Naming, units, and scenario conventions.
  coefficients.yaml  Wilson-coefficient labels and flavour patterns.
  operator-map.yaml   LFU profiler names mapped to analysis and plotting labels.
  datasets.yaml      Dataset and projection labels.

results/
  cms-current/       Current CMS high-mass dilepton results.
  hl-lhc/            HL-LHC sensitivity projections.
```

The result directories are organized by physics scenario and analysis setup. Empty directories are retained with `.gitkeep` files until numerical tables are added.

## Result categories

- `wy`: flavour-universal `W` and `Y` parameter scenario.
- `lfu`: lepton-flavour-universal SMEFT scenario with resolved quark flavour.
- `flavour-general`: separate electron and muon coefficient fits.

Dataset labels:

- `cms-current`: current CMS Run-II high-mass dilepton data.
- `hl-lhc`: high-luminosity LHC projections.

HL-LHC setup labels:

- `angular`: results using the two Collins-Soper angular bins.
- `no-angular`: results after merging angular bins.
- `rsyst-0p2`: projected systematic covariance scaled by `r_syst = 0.2`.
- `rsyst-1p0`: projected systematic covariance scaled by `r_syst = 1.0`.

## Citation

Please cite the paper associated with this repository. The final arXiv, DOI, and journal information will be added once available.
