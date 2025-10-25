# amogh-et-al-ssq-cf-fermi-sea

Static structure factor datasets for composite-fermion (CF) Fermi-sea
wavefunctions. Each CSV is named `ssq_N{N}_2Q{2Q}.csv`, where `N` is the
number of particles in the simulation and `2Q` is the total flux.

The repository currently contains data for the following system sizes:

```
ssq_N81_2Q80.csv    ssq_N81_2Q160.csv   ssq_N81_2Q240.csv   ssq_N81_2Q320.csv
ssq_N200_2Q496.csv  ssq_N225_2Q448.csv  ssq_N256_2Q510.csv  ssq_N289_2Q1152.csv
ssq_N300_2Q746.csv  ssq_N324_2Q323.csv  ssq_N324_2Q969.csv  ssq_N324_2Q1292.csv
ssq_N361_2Q720.csv  ssq_N361_2Q1440.csv ssq_N400_2Q399.csv  ssq_N400_2Q798.csv
ssq_N400_2Q996.csv  ssq_N400_2Q1197.csv ssq_N400_2Q1596.csv ssq_N484_2Q483.csv
ssq_N484_2Q1449.csv ssq_N484_2Q1932.csv ssq_N576_2Q575.csv  ssq_N576_2Q1725.csv
ssq_N576_2Q2300.csv ssq_N625_2Q624.csv  ssq_N625_2Q1248.csv ssq_N900_2Q899.csv
ssq_N900_2Q1798.csv
```

## Column definitions

Each CSV is comma-separated with a header row:

- `k`: wavevector magnitude measured in units of \(1/\ell_B\).
- `L`: angular momentum quantum number on the sphere.
- `S`: unprojected static structure factor \(S(q)\).
- `Sbar`: projected static structure factor \(\bar{S}(q)\); this may be
  `NaN` when projection is unavailable for a given dataset.
- `std(S)`: one-sigma uncertainty for the corresponding structure-factor
  entry; treat it as the error bar on \(S(q)\) or \(\bar{S}(q)\).

## Citation requirement

Use the data however you like, but if you publish results that rely on
these files you must cite the accompanying paper by Amogh et al. (provide
the appropriate bibliographic information in your work).
