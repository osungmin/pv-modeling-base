# ☀️⚡ PV Modeling Base

Core scripts for my ongoing PV modeling research.

This repository contains reusable components for preparing data, engineering features, and building baseline PV performance and capacity‑factor models.

Here you'll find:
- Data preparation & preprocessing routines
- Irradiance/temperature handling
- Feature engineering for PV performance modeling
- Baseline modeling and evaluation

Basically, everything I keep reusing whenever I start a new PV experiment.


## Repository Structure
```
pv-modeling-base/
├── data_preprocessing/
│   ├── asos_agg.py
│   ├── aws_agg.py
│   └── airk_agg.py 
│   └── kpx.py
├── modeling/
│   ├── global_attenuation_model_v1.py
│   └── cf_model_tuning_v1.py
│   └── global_cf_model_v1.py
├── shap/ 
└── README.md
```


## Data Preprocessing Modules

Scripts under data_preprocessing/ handle regional-level aggregation and transformation of weather and operational datasets used in PV modeling.

- ASOS/AWS data source: Korea Meteorological Administration (KMA) Open Data Portal – [https://data.kma.go.kr/](https://apihub.kma.go.kr/)
- AIRK PM data source: National Institute of Meteorological Sciences (NIMS) – [https://apihub.kma.go.kr/](https://www.airkorea.or.kr/)
- KPX Operational PV data source: KPX Open Data Portal – [[https://epsis.kpx.or.kr](https://www.data.go.kr/data/15065269/fileData.do)
- Regional shapefiles: GADM (gadm41_KOR_1) – https://gadm.org/data.html

## Usage

Each script is modular, so you can run them independently depending on which part 
of the PV workflow you're working on.

