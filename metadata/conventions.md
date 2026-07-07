# Conventions

This file defines the labels used throughout the ancillary result archive.

## Paths

- Use lowercase directory names.
- Use hyphenated labels for multi-word categories.
- Organize result files by dataset, physics scenario, angular treatment, and systematic benchmark.
- Keep numerical data in `results/`; keep descriptive metadata in `metadata/`.

## Operator names

- Future LFU result files should use `profiler_name` as the canonical machine key.
- The operator-name chain is `profiler_name -> analysis_label -> plot_label_tex`.
- `profiler_name` is the exact name used by the profiling code and operator directories, for example `C_Q1_L_P`.
- `analysis_label` is the intermediate label stored in profiler summaries, for example `ClqP[ll,ll,1,1]`.
- `plot_label_tex` is the paper-facing plotting label, for example `C_{lq}^{(+)[\ell\ell 11]}`.
- The full LFU lookup table is stored in `metadata/operator-map.yaml`.

## Units

- Wilson coefficients are expressed in `TeV^-2`.
- The universal `W` and `Y` parameters are dimensionless.
- Dilepton invariant masses are expressed in `GeV`.
- Luminosities are expressed in `fb^-1` or `ab^-1`, as stated in the relevant metadata.

## Statistical convention

- Quoted one-parameter intervals are 95% CL intervals.
- The default one-parameter threshold is `Delta chi^2 = 3.84`.
- Two-parameter contours use the 95% CL threshold `Delta chi^2 = 5.99`.
- Bounds are reported with respect to the profiled best-fit point unless otherwise stated.

## Dataset labels

- `cms-current`: current CMS Run-II high-mass dilepton dataset at `sqrt(s) = 13 TeV`.
- `hl-lhc`: high-luminosity LHC projection at `sqrt(s) = 14 TeV`.

## Scenario labels

- `wy`: flavour-universal `W` and `Y` parameter scenario.
- `lfu`: lepton-flavour-universal SMEFT scenario.
- `flavour-general`: flavour-general SMEFT scenario with separate electron and muon coefficients.

## Analysis setup labels

- `angular`: the two Collins-Soper angular bins are kept separate.
- `no-angular`: Collins-Soper angular bins are merged.
- `rsyst-0p2`: HL-LHC systematic covariance benchmark with `r_syst = 0.2`.
- `rsyst-1p0`: HL-LHC systematic covariance benchmark with `r_syst = 1.0`.

## PDF-treatment labels

- `fixed`: PDF nuisance parameters are fixed to their central values.
- `profiled`: PDF nuisance parameters are profiled in the likelihood.
