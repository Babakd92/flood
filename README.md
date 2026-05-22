# 14-Day Flood Prediction for Huron River, Ohio

This repository runs daily Random Forest flood prediction models for the Huron River and Sandusky River watersheds and generates an interactive forecast dashboard.

## Main Files

- `version_8.py` - daily flood prediction model and dashboard generator
- `input_huron.csv` - historical daily water-level and precipitation input data for Huron River
- `input_sandusky.csv` - historical daily water-level and precipitation input data for Sandusky River
- `Watershed Shapefile/Huron River/data.geojson` - Huron River watershed boundary used in the interactive map
- `Watershed Shapefile/Sandusky River/download/layers` - Sandusky River watershed shapefile used in the interactive map
- `index.html` - generated interactive dashboard for GitHub Pages
- `requirements.txt` - Python dependencies for GitHub Actions
- `.github/workflows/daily-flood-forecast.yml` - scheduled GitHub Actions workflow

## Automation

GitHub Actions runs the model every day at 1:00 AM Eastern during daylight saving time, regenerates the dashboard and output files, and commits updated outputs back to the repository.

The workflow can also be started manually from the repository's Actions tab.
