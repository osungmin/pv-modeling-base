# PV Modeling Base

Core scripts for my ongoing PV modeling research.

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
└── README.md
```



## Usage

Each script is modular, so you can run them independently depending on which part 
of the PV workflow you're working on.

