# Forest Fire Danger Index & Koala Habitat Analysis – Queensland

This project evaluates forest fire risk in Queensland, Australia and its impact on koala habitats (2013–2023). It replicates a study from New South Wales, calculating the **Forest Fire Danger Index (FFDI)** using climatic data, analyzing **spatio-temporal fire patterns** through harmonic regression and clustering, and assessing exposure of **high-suitability koala habitat** to fire danger.

---

## 📂 Data

**Required data:**  
- ERA5: Daily maximum temperature & precipitation  
- TerraClimate: Monthly wind speed & mean temperature  
- Koala habitat model (ArcGIS Pro)  
- Queensland administrative boundaries  

> Download all data from [https://drive.google.com/drive/folders/1QjXXoZuTgwmj2dZJMiwF0OdpIznDoPiV?usp=sharing] and place in a `Data/` folder **next to notebooks**.

**Formats:** GeoTIFF (`.tif`), Shapefile/GeoPackage (`.shp`/`.gpkg`), CSV (`.csv`)

---

## 📝 Notebooks (Run in order)

1. `1. KBDI Calculation.ipynb`  
2. `2. Drought Factor Computation.ipynb`  
3. `3. FFDI_Calculation.ipynb`  
4. `4. Calculation of high risk areas.ipynb`  
5. `5. FFDI Spatio-Temporal Analysis.ipynb`  
6. `6. Koala Preprocessing .ipynb`  
7. `7. Overlap Analysis FFDI Koala Habitat.ipynb`  

---

## ⚡ Usage

1. Place the `Data/` folder in the same directory as the notebooks.  
2. Open each notebook in order and run all cells.  
3. Outputs (maps, plots, processed rasters) will be saved in `Outputs/`.

---

## 🧰 Tools & Libraries

- Python 3.x, Jupyter Notebook  
- `numpy`, `pandas`, `rasterio`, `geopandas`, `matplotlib`  
- `scipy`, `pymannkendall`  

---

## 📜 Notes

- All data is secondary environmental data; no ethical approval required.  
- Scripts are version-controlled for reproducibility.  
- ArcGIS Pro is needed to access raw koala habitat data.
