# Climate Math Research

Quantifying Equilibrium Climate Sensitivity (ECS) using a zero-dimensional energy balance model. This project estimates how much Earth's global mean surface temperature would rise if atmospheric CO2 concentrations were to double, based on observed CO2 and temperature data from 1994–2024.

Group project for MATH 586: Climate Mathematics, San Diego State University.

## Authors

- Christian Byars
- Lillian Snyder
- Jonathan Siegel
- Alexander Grimes

## Setup

Requires Python 3.12 and [uv](https://docs.astral.sh/uv/).

```bash
git clone https://github.com/ChristianByars/Climate-Math-Research.git
cd Climate-Math-Research
uv sync
```

## Usage

Open `climate_ecs_analysis.ipynb` in your preferred IDE and run the cells. All figures are saved to the `figures/` directory.

## Project Structure

```
├── climate_ecs_analysis.ipynb   # Main analysis notebook
├── co2_mm_mlo.csv               # Mauna Loa CO2 monthly means (1958–2025)
├── GLB.Ts+dSST.csv              # GISTEMP global temperature anomalies (1880–2025)
├── NOAAGlobalTemp_v6.1.0_...nc  # NOAA GlobalTemp v6.1.0 gridded anomalies (1850–2026)
├── figures/                     # Generated figures (PNG)
├── pyproject.toml               # Project dependencies
└── uv.lock                     # Dependency lock file
```

## Data Sources

- **CO2**: NOAA Global Monitoring Laboratory, Mauna Loa monthly mean CO2 concentrations
- **Temperature**: NASA Goddard Institute for Space Studies (GISTEMP v4), global mean surface temperature anomalies relative to the 1951–1980 baseline
- **Temperature (validation)**: NOAA GlobalTemp v6.1.0, gridded global temperature anomalies (ERSSTv6 + GHCNm v4)
