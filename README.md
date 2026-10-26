# Gut-Brain Modules (GBMs) – companion website and supplementary data

Companion website and supplementary data for:

> Valles-Colomer M, Falony G, Darzi Y, Tigchelaar EF, Wang J, Tito RY, Schiweck C, Kurilshikov A, Joossens M, Wijmenga C, Claes S, Van Oudenhove L, Zhernakova A, Vieira-Silva S, Raes J. **The neuroactive potential of the human gut microbiota in quality of life and depression**. *Nature Microbiology* 4(4):623–632 (2019). [doi:10.1038/s41564-018-0337-x](https://doi.org/10.1038/s41564-018-0337-x)

It contains the database of manually curated gut-brain modules (GBMs). Each GBM corresponds to a single neuroactive compound production or degradation process.

**Website:** https://raeslab.github.io/GBMs/ (GitHub Pages, served from `docs/` on the `main` branch)

This material was previously hosted on the Raes Lab website at `raeslab.org/software/gbms.html` and has been migrated to this repository.

## Contents

| Path | Size | Description |
|------|------|-------------|
| `supplementary/GBMs.zip` | 6 KB | Archive with all supplementary files |
| `supplementary/GBMs/GBM.inputfile.txt` | 5 KB | GBM definitions reduced to module id, name and orthologue sets per step (module database input format, e.g. for omixer-rpm). |
| `supplementary/GBMs/Supplementary.Data.S1.txt` | 11 KB | Full GBM definitions: module id and name, input/output compounds, orthologue (KO/COG) sets per step and literature references. |

Total supplementary data: 22 KB.

## Repository layout

```
docs/                 Static, self-contained website (GitHub Pages source; no external CSS/JS/fonts)
  index.html
  assets/             Stylesheet, script, logo, figure previews
supplementary/        Downloadable data files (Git LFS)
.gitattributes        Git LFS tracking rules
```

### Git LFS

All files in `supplementary/` are tracked with [Git LFS](https://git-lfs.com). Install it before cloning
(`git lfs install`), or download individual files from the website. Because GitHub Pages does not serve LFS
objects, the website's download buttons point to `https://github.com/raeslab/GBMs/raw/main/supplementary/...`;
when `docs/index.html` is opened from a local checkout the links switch to the relative `../supplementary/` paths.

### Publishing

In the repository settings, enable GitHub Pages with source *Deploy from a branch* → `main` / `/docs`.

## How to cite

If you use these data, please cite:

> Valles-Colomer M, Falony G, Darzi Y, Tigchelaar EF, Wang J, Tito RY, Schiweck C, Kurilshikov A, Joossens M, Wijmenga C, Claes S, Van Oudenhove L, Zhernakova A, Vieira-Silva S, Raes J. **The neuroactive potential of the human gut microbiota in quality of life and depression**. *Nature Microbiology* 4(4):623–632 (2019). [doi:10.1038/s41564-018-0337-x](https://doi.org/10.1038/s41564-018-0337-x)

```bibtex
@article{vallescolomer2019neuroactive,
  title   = {{The neuroactive potential of the human gut microbiota in quality of life and depression}},
  author  = {Valles-Colomer, M. and Falony, G. and Darzi, Y. and Tigchelaar, E. F. and Wang, J. and Tito, R. Y. and Schiweck, C. and Kurilshikov, A. and Joossens, M. and Wijmenga, C. and Claes, S. and Van Oudenhove, L. and Zhernakova, A. and Vieira-Silva, S. and Raes, J.},
  journal = {Nature Microbiology},
  year    = {2019},
  volume  = {4},
  number  = {4},
  pages   = {623--632},
  doi     = {10.1038/s41564-018-0337-x}
}
```

## Contact

Raes Lab, VIB–KU Leuven Center for Microbiology – Prof. Jeroen Raes (jeroen.raes@kuleuven.be).
