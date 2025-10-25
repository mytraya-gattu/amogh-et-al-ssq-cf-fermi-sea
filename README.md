# amogh-et-al-ssq-cf-fermi-sea

Static structure factor datasets for composite-fermion (CF) Fermi-sea
wavefunctions. Each CSV is named `ssq_N{N}_2Q{2Q}.csv`, where `N` is the
number of particles in the simulation and `2Q` is the total flux.

The repository currently contains data for the following system sizes,
reported by particle number \(N\), monopole strength \(2Q\), and filling
factor \((N-1)/(2Q)\) expressed as a rational number:

| `N` | `2Q` | \((N-1)/(2Q)\) |
| --- | --- | --- |
| 81 | 80 | 1/1 |
| 81 | 160 | 1/2 |
| 81 | 240 | 1/3 |
| 81 | 320 | 1/4 |
| 225 | 448 | 1/2 |
| 256 | 510 | 1/2 |
| 289 | 1152 | 1/4 |
| 324 | 323 | 1/1 |
| 324 | 969 | 1/3 |
| 324 | 1292 | 1/4 |
| 361 | 720 | 1/2 |
| 361 | 1440 | 1/4 |
| 400 | 399 | 1/1 |
| 400 | 798 | 1/2 |
| 400 | 1197 | 1/3 |
| 400 | 1596 | 1/4 |
| 484 | 483 | 1/1 |
| 484 | 1449 | 1/3 |
| 484 | 1932 | 1/4 |
| 576 | 575 | 1/1 |
| 576 | 1725 | 1/3 |
| 576 | 2300 | 1/4 |
| 625 | 624 | 1/1 |
| 625 | 1248 | 1/2 |
| 900 | 899 | 1/1 |
| 900 | 1798 | 1/2 |
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
these files you must cite the accompanying paper by Amogh et al.: Exploring the nature of the emergent gauge field in composite-fermion metals: A large-scale microscopic study.
