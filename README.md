# Blockades, Flag Mimicry, and Grain Lifelines: Physical Anatomy of Russian and Baltic Maritime Trade in the Sound Toll Registers, 1700–1856

[![License: MIT](https://shields.io)](LICENSE)

This repository contains the complete archival pre-auditing pipeline, orthographic normalization rules, reproducible Python/Jupyter code, high-resolution figures, and LaTeX manuscript sources for the study:

> **Avtonomov, P. (2026).** *Blockades, Flag Mimicry, and Grain Lifelines: Physical Anatomy of Russian and Baltic Maritime Trade in the Sound Toll Registers, 1700–1856.*

This work is the second study in an empirical research cycle examining the physical and financial mechanisms of early modern and modern market integration, building directly on our preceding price-chronicle audit (`doi:10.5281/zenodo.24436177`).

## Key Empirical Findings
* **Archival Pre-Audit (`1700–1856`):** Screening `1,274,843` unique ship passages and `3,637,322` cargo records in the Sound Toll Registers Online (`STRO`) resolves eighteenth-century Danish-German spelling variants (e.g., `Petersborg` / `St. Petersborg`, `Dantzig` / `Danschen`, `Rug` / `Rugh`) and establishes a continuous 135-year benchmark panel (`1722–1856`) following the Treaty of Nystad (`1721`).
* **Geopolitical Chokepoint Localization vs. Peacetime Structure:** Across 20 major ports (`1722–1856`), `37.9%` of annual log-growth variance is tightly localized in physical chokepoint closures during the Napoleonic Continental Blockade (`1808`: `36.8%`; `1814` rebound: `17.5%`) and the Crimean War (`1854–1856`), yielding $\mathrm{PR}(u_1) = 0.033$. Removing wartime blockades reduces Mode 1 variance to `20.8%` ($\mathrm{PR}(v_1) = 0.539$) and reveals a structural polarity (`Mode 2`, `12.6%`) separating a *Russian–British industrial-naval belt* (`St. Petersburg`, `Riga`, `Narva`, `Vyborg`, `London`, `Hull`) from a *Prussian–Dutch–French grain and wine belt* (`Gdansk`, `Stettin`, `Amsterdam`, `Rotterdam`, `Bordeaux`).
* **Wartime Flag Adaptation:** Shipmaster homeport records document the drop in British clearances from St. Petersburg and Riga from `648` in 1806 to `0` in 1808 and 1811–1812, bridged tactically by neutral U.S. shipping in 1810–1811 and followed by a sixfold post-1814 surge in Russian Baltic-registered vessels.
* **From Eighteenth-Century Supply Contractions to Nineteenth-Century Grain Lifelines:** During eighteenth-century European subsistence crises (`1741`, `1771`, `1795`), physical grain clearances fell sharply to `204–436` ships/year (below the `774`-ship mean). In the nineteenth century, Baltic and Russian ports acted as elastic supply lifelines, dispatching `2,630` grain ships in `1817` and `3,263` ships in `1847` (led by `1,275` clearances from St. Petersburg).

## Repository Structure
* `reproduce_stro_study.ipynb` — End-to-end Jupyter Notebook reproducing all archival audits, summary statistics, and figures.
* `reproduce_stro_study.py` — Standalone Python script version of the pipeline.
* `Figure_1_STRO.png`, `Figure_2_STRO.png`, `Figure_3_STRO.png` — High-resolution (300 dpi) multi-panel figures.
* `paper/main.tex` — Complete LaTeX source file for the manuscript.
* `data/README.md` — Instructions for downloading the raw `STRO` archives (`doorvaarten.csv.zip` and `ladingen.csv.zip`).

## How to Reproduce
1. Download the relational CSV exports (`doorvaarten.csv.zip` and `ladingen.csv.zip`) from the [Sound Toll Registers Online (STRO)](https://soundtoll.nl) portal and place them in the root directory (or `data/`).
2. Run `reproduce_stro_study.ipynb` (or `python reproduce_stro_study.py`) to extract the archives, run the pre-audit and two-tier spectral diagnostics, and regenerate all summary metrics and figures.
