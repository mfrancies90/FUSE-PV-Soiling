# FUSE-PV-Soiling
# FUSE — Fusion for Understanding Soiling Events

A data-driven framework for daily photovoltaic soiling prediction in Egypt
using multi-source open-access reanalysis data. Two-level fusion: (i) data
fusion across PVGIS/SARAH-3, ERA5, and CAMS EAC4, and (ii) model fusion via
a weighted soft-voting ensemble of Random Forest, XGBoost, and LightGBM.

## Highlights
- Unified daily dataset of 3,652 records covering Cairo and Aswan (2019–2023).
- Twenty input variables fused from three open-access geophysical sources.
- Unsupervised K-Means labeling on Dust AOD produces parameter-free
  CLEAN / SOILED labels (boundary ≈ 0.1666).
- Weighted soft-voting ensemble (RF + XGBoost + LightGBM) achieves
  weighted F1 > 90% and AUC-ROC > 0.96 on the held-out 2023 test year.
- Feature-importance and ablation studies confirm PM10 and humidity-
  persistence as dominant soiling drivers.

## Data Sources
- **PVGIS / SARAH-3** — solar resource and PV power (EU JRC).
- **ERA5** — meteorological reanalysis (ECMWF / Copernicus CDS).
- **CAMS EAC4** — atmospheric composition reanalysis (ECMWF / Copernicus ADS).

## Repository Structure
- `notebooks/` — end-to-end pipeline and per-source EDA notebooks.
- `data/` — pointers to source datasets (raw files not redistributed).
- `figures/` — publication figures.

