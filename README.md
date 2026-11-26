# Tonale school: multimessenger cosmology

Working-group material for the lectures *Cosmological probes of the dark sector* (V. Poulin).

- `working_groups.pdf`: the exercise sheet, one part per lecture (Discuss, Estimate and Notebook items).
- `notebooks/`: the three notebooks used by the sheet, with their precomputed tables in `notebooks/data/`.
  - `NB1_dark_matter_models.ipynb`: dark matter in the CMB and in P(k); warm, ultralight and decaying dark matter.
  - `NB2_neutrinos_Neff.ipynb`: neutrino masses and extra relativistic species.
  - `NB3_energy_injection.ipynb`: dark matter annihilations and decays in the thermal history.

## Running the notebooks

Python 3 with `numpy`, `scipy`, `matplotlib` and `jupyter`. The notebooks call CLASS through `classy`:

```bash
pip install numpy scipy matplotlib jupyter classy
```

The ultralight scalar field needs AxiCLASS (CLASS with a scalar field): clone
https://github.com/PoulinV/AxiCLASS and run `make`. Without CLASS, the notebooks fall back on the tables in
`notebooks/data/`.

Run them from the `notebooks/` folder, so that the relative paths to `data/` work:

```bash
cd notebooks
jupyter notebook
```
