# INF201 - Deliverable 1: Weather data from Ås

Analysis of weather data from the Ås weather station (SN17850), collected from
the Norwegian Meteorological Institute through the [Frost API](https://frost.met.no).

All code, plots and discussion are in [`deliverable_1.ipynb`](deliverable_1.ipynb).

## Contents

| Task | Description |
|------|-------------|
| 1 | Daily mean air temperature in 2025: plot and summary table |
| 2 | Temperature and daily precipitation in the same plot |
| 3 | Comparison of 2025 with 1925 (100 years earlier) |
| 4 | Function that counts heatwaves for any station and year and writes a yml summary |
| 5 | Function for the 7-day moving average of temperature |

## Files

- `deliverable_1.ipynb` - the notebook with code, results and discussion
- `heatwave_summary.yml` - heatwave summary for Ås in 2025 (output of task 4)
- `heatwave_summary_example.yml` - example of the yml format given in the assignment

## How to run

1. Install the packages:
   ```
   pip install requests pandas matplotlib pyyaml jupyter
   ```
2. Create a user at [frost.met.no](https://frost.met.no/auth/requestCredentials.html)
   to get a client ID.
3. Make a file called `api.txt` in the same folder as the notebook, with this line:
   ```
   client id: <your-client-id>
   ```
   This file is in `.gitignore` and should never be committed.
4. Open the notebook and run all cells.

## References

- MET Norway, Frost API Python example: https://frost.met.no/python_example.html
