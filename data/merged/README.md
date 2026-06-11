# Data

## Processed (included in repo)
- `merged/clean_data_2019_2023.csv` — 3,652 daily records, 20 variables,
  Cairo & Aswan, 2019–2023.
- `merged/train_binary.csv` — training subset (2019–2022).
- `merged/test_binary.csv`  — test subset (2023).

## Raw (NOT in repo — download from source)
- **PVGIS / SARAH-3**: https://re.jrc.ec.europa.eu/pvg_tools/en/
- **ERA5**: https://cds.climate.copernicus.eu  (search for *ERA5 single levels*)
- **CAMS EAC4**: https://ads.atmosphere.copernicus.eu  (search for *EAC4*)

Drop the downloaded files into `data/raw/` to reproduce the pipeline.
