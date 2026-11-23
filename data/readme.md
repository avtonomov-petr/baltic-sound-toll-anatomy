# Raw Data Instructions: Sound Toll Registers Online (STRO)

Due to GitHub file size limits, the raw compressed relational archives (`doorvaarten.csv.zip`, ~66.5 MB, and `ladingen.csv.zip`, ~73.9 MB) are not hosted directly in this repository.

## How to Obtain the Raw Data

1. Visit the official **Sound Toll Registers Online (STRO)** portal maintained by the University of Groningen and DANS:  
   **https://soundtoll.nl**
2. Navigate to the **Data / Download** section and download the complete relational CSV export containing:
   - `doorvaarten.csv` (individual vessel passages through the Øresund, 1497–1857)
   - `ladingen.csv` (commodity cargo entries linked via `id_doorvaart`)
3. Place `doorvaarten.csv.zip` and `ladingen.csv.zip` either in the root directory of this repository or inside this `data/` folder.
4. Run `reproduce_stro_study.ipynb` (or `python reproduce_stro_study.py`). The script will automatically extract the CSV tables, apply the orthographic normalization and deduplication pipeline, and reproduce all summary statistics and 300 dpi figures.

## Citation for the Underlying Dataset
Veluwenkamp, J. W., & Scheltjens, W. (Eds.). (2018). *Early modern shipping and trade: Novel approaches using Sound Toll Registers Online*. Brill. Data portal: https://soundtoll.nl

