# amogh-et-al-ssq-cf-fermi-sea

Static structure factor datasets for composite-fermion (CF) Fermi-sea
wavefunctions. Each CSV is named `ssq_N{N}_2Q{2Q}.csv`, where `N` is the
number of particles in the simulation and `2Q` is the total flux.

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
