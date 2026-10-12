## Weather
Title: Weather data analysis comparing precipitation in Seattle, WA and Miami, FL from 2018-2022


## Introduction
---
I want to compare the patterns of precipitation between two cities. I chose Miami because I was interested in whether South Florida's hurricane and wet seasons would result in Miami actually receiving more rainfall than Seattle. 

## Project Overview

This project compares precipitation data from Seattle, Washington and Miami, Florida from 2018 to 2022 to determine which city receives more rainfall.

Objective: Compare rainfall amount and frequency between Seattle and Miami.

Domain: Weather and climate

Key techniques: Data cleaning, filtering, merging, reshaping, missing-value handling, visualization, Welch's two-sample t-tests, and two-proportion z-tests.

The main finding was that Seattle experiences precipitation more frequently during much of the year, while Miami tends to receive greater amounts of precipitation during its wetter months.


---

## Project Structure

Weather/
├── data/
│   ├── seattle_rain.csv
│   ├── miami_rain.csv
│   └── clean_seattle_miami_weather.csv
├── code/
│   └── WeatherData.ipynb
├── Seattle_Miami_Weather_Report.pdf
├── README.md
├── requirements.txt
└── LICENSE

---

## Data

Source: NOAA Climate Data Online and the DATA 5100 course GitHub repository.

Description: Daily precipitation data for Seattle, Washington and Miami, Florida from January 1, 2018 through December 31, 2022. The data are stored in CSV format and include fields such as date, weather station, and precipitation.

Seattle Data Source:
https://www.ncei.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:US1WAKG0204/detail

Miami Data Source:
https://www.ncei.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USW00092811/detail

NOAA climate data are publicly available for research and educational use.

---

## Analysis

The datasets were inspected, cleaned, and filtered to the desired date range. Missing values were identified and handled, and the Seattle and Miami datasets were combined into a tidy format for analysis.

Derived variables were created for month, season, and whether precipitation occurred on a given day. The analysis used summary statistics and visualizations to compare precipitation amount and frequency between the two cities. Welch's two-sample t-tests were used to compare mean daily precipitation by month, and two-proportion z-tests were used to compare the proportion of days with precipitation.

Analysis notebook:
`code/WeatherData.ipynb`

Clean data file:
`data/clean_seattle_miami_weather.csv`

---

## Results

Welch's two-sample t-tests showed statistically significant differences in mean daily precipitation during several months of the year. Seattle had greater mean precipitation during parts of the winter, while Miami had substantially greater precipitation during the late spring and summer months.

The two-proportion z-tests showed that Seattle experienced precipitation on more days during most months from 2018–2022.



## Conclusion

The results show that saying "Seattle gets more rain" than Miami can be misleading. Seattle generally experiences rain more frequently, especially during the cooler months, while Miami tends to receive heavier rainfall during its wet season.

Whether Seattle is considered rainier depends on whether rainfall is measured by frequency or total precipitation amount.


---

## Authors

- Hakim Mims - https://github.com/HakimMims

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

Tools/libraries used: Python, JupyterLab, pandas, NumPy, Matplotlib, Seaborn, SciPy, and statsmodels.

Tutorials or papers referenced: DATA 5100 course materials and NOAA Climate Data Online documentation.

Project structure and workflow were based on DATA 5100 course examples and instructor guidance.