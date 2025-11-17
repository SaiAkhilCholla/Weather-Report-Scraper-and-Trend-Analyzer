## 📈 Weather Report Scraper and Trend Analyzer

This project provides an end-to-end Python pipeline for processing historical weather data, summarizing key metrics, and visualizing daily and seasonal trends.

-----

## 🎯 Project Overview

This tool transforms raw, time-series weather data (likely hourly or sub-daily) into structured daily and monthly summaries. The primary goal is to derive meaningful insights into the **seasonal patterns** and **extreme event occurrences** for the specified location (implied to be Hyderabad).

### Key Features

  * **Data Cleaning:** Converts timestamps, selects core variables, and renames columns for clarity.
  * **Time-Series Aggregation:** Calculates daily metrics (Total Rainfall, Max Wind Speed, Avg Temperature/Humidity).
  * **Seasonal Analysis:** Computes long-term average monthly statistics.
  * **Visualization:** Generates informative charts displaying both short-term daily volatility and long-term seasonal cycles.

-----

## 🛠️ Requirements

To run this analysis, you must have Python installed, along with the following libraries:

```bash
pip install pandas matplotlib seaborn
```

### Input Data

The analysis requires a CSV file named `hyderabad.csv` to be present in the same directory as the script. The file must contain at least the following columns:

| Column Name | Description |
| :--- | :--- |
| `date_time` | Timestamp of the recording (required for indexing and resampling). |
| `tempC` | Temperature in Celsius. |
| `precipMM` | Precipitation in millimeters. |
| `windspeedKmph` | Wind speed in kilometers per hour. |
| `humidity` | Relative humidity percentage. |

-----

## 🚀 How to Run the Program

1.  **Save the Code:** Save the provided Python script (the code block from the prompt) as `weather_analyzer.py`.

2.  **Place Data:** Ensure the `hyderabad.csv` file is in the same directory as `weather_analyzer.py`.

3.  **Execute:** Run the script from your terminal:

    ```bash
    python weather_analyzer.py
    ```

-----

## 🖼️ Output Files

The script generates two main visualization images, which will be saved in the same directory:

| File Name | Description |
| :--- | :--- |
| **`daily_trends_rainfall_wind.png`** | Line plots showing the daily total rainfall and maximum wind speed across the entire data period, highlighting specific weather events. |
| **`monthly_seasonal_trends.png`** | A 2x2 grid of plots showing the average monthly cycle for Temperature, Rainfall, Wind Speed, and Humidity, revealing seasonal patterns. |

-----

## 🤝 Contribution

This project was developed by **Sai Akhil Cholla And Vardhan Reddy Mallidi**.
