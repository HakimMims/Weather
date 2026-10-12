## Weather
Title: Weather data analysis comparing precipitation in Seattle, WA and Miami, FL from 2018-2022


## Introduction
---
I want to compare the patterns of precipitation between two cities. I chose Miami because I was interested in whether South Florida's hurrcane and wet seasons would result in Miami actually receiving more rainfall than Seattle. 

## Project Overview

This project compares precipitation data from Seattle, Washington and Miami, Florida from 2018 to 2022 to determine which city receives more rainfall.

Object: Daily rainfall data
Domain: Weather and climate
Key techniques: Data cleaning, filtering, merging, reshaping, missing-value handling, and visualization with Python/pandas.

---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

Source: NOAA Climate Data Online and the DATA 5100 course GitHub repository

Description: Daily precipitation data for Seattle, Washington and Miami, Florida from January 1, 2018 through December 31, 2022. The data are stored in CSV format and include fields such as date, weather station, and precipitation.

License: NOAA climate data are publicly available for research and educational use

---

## Analysis

Compare precipitation patterns between Seattle and Miami from 2018–2022 using summary statistics and visualizations. This may include comparing total rainfall, average daily precipitation, and the number of rainy days in each city.
---

## Results

To compare rainfall patterns between Seattle and Miami, I used Welch's two sample t- test to assess differences in mean daily precipitation by month. Two proportion z tests were used to compare the proportion of days with precipitation between the two cities.

The analysis showed statistically significant differences in mean daily precipitation during several months of the year. Seattle proved to have greater mean precipiation during parts of the winter, whereas Miami had substantially greater precipiation during late spring and summer months. 

The proportion tests showed Seattle experienced precipitation on more days during most of the months during 2018-2022


## Conclusion

The results show saying "Seattle gets more rain" than Miami is quite misleading. The results show Seattle generally experiences rain more frequenty, especially during the coler months, while Miami tends to recieve heavier rainfall during its wet season. Therefore, whether Seattle is considered more rainier depends on whether rainfall is measured by frequency or the total amount. 

---

## Authors

- Hakim Mims - https://github.com/HakimMims

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

Tools/libraries used: Python, JupyterLab, pandas, NumPy, Matplotlib, and Seaborn

Tutorials or papers referenced: DATA 5100 course materials and NOAA Climate Data Online documentation

Inspiration or collaborators: Project structure and workflow based on DATA 5100 course examples and instructor guidance