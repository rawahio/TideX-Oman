# TideX: Protecting Water Security from Space

Early warning of harmful algal blooms (red tides) for desalination plants, built with NASA satellite data.
NASA Space Apps Challenge 2026, Team TideX, Oman.

Demo video (30 s): https://youtu.be/BfGg7Q1dRgI

## What it does
TideX detects algal blooms from NASA MODIS-Aqua chlorophyll-a, measures how far each bloom is from six desalination plants in Oman, and uses NASA OSCAR ocean currents to estimate whether the bloom is drifting toward a plant and when it would arrive. Warning at 50 km, critical at 20 km. Arabic and English, interactive map, crisis timeline and PDF report.

## Tested on the real 2008 red tide
Replayed on real NASA data (October to December 2008): TideX flagged a bloom near Barka on 22 October, 25 days before it reached the coast on 16 November.

## How to run it
1. Download `TideX_Oman_project.zip` from this page and unzip it.
2. Open a terminal inside the unzipped folder and install the libraries:
   pip install streamlit pandas numpy plotly fpdf2 uharfbuzz xarray netcdf4 global-land-mask scipy
3. Start the app:
   streamlit run app.py
4. In the sidebar choose "2008 crisis replay (NASA data)".

## NASA data used
- MODIS-Aqua Level-3 daily chlorophyll-a, 4 km (OB.DAAC)
- MODIS-Aqua Level-3 daily sea surface temperature, 4 km (OB.DAAC)
- OSCAR surface currents v2.0, 0.25 degree (PO.DAAC)

## Acknowledgements
Faculty of the Department of Marine Science and Fisheries, Sultan Qaboos University, and staff at desalination plants in Oman who shared their experience with red tides.

## Use of AI tools
An AI assistant (Claude) helped write and debug parts of the code and produce the video graphics and subtitles. The idea, the 2008 case study, the data choices and the narration are the team's own.
