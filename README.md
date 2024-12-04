
# Daily AQI Comparison for Ahmedabad

This project compares the officially reported daily AQI values for Ahmedabad with manually calculated daily AQI values. The manual calculation is performed by taking the average of hourly AQI data.

## Project Overview

Air Quality Index (AQI) is an essential metric for understanding air pollution levels. This project aims to verify the accuracy of officially reported daily AQI by comparing it with manually computed averages of hourly AQI data for the same period.

## Data Sources

- **Official AQI Data**: Downloaded from the [Central Pollution Control Board (CPCB) AQI Repository](https://cpcb.nic.in/aqi-bulletin-3/).
- **Hourly AQI Data**: Hourly AQI data for Ahmedabad, extracted from the monthly Excel files available on the [CPCB portal](https://airquality.cpcb.gov.in/ccr/#/caaqm-dashboard-all/caaqm-landing/aqi-repository).

## Methodology

1. **Data Extraction**:
    - The hourly AQI data is downloaded in Excel format for each month of 2023.
    - Official daily AQI values are also retrieved for comparison.

2. **Manual AQI Calculation**:
    - For each day, the hourly AQI values are averaged to compute the daily AQI.
    - Special care is taken to handle missing or incomplete data by filling NaN values with the average of the respective column.

3. **Comparison**:
    - Both datasets (official and manually calculated) are compared to identify discrepancies and patterns.

4. **Visualization**:
    - Plots are generated to visually compare the two datasets.
    - Differences between the two values are highlighted.

## Prerequisites

- Python 3.8 or higher
- Required Python libraries: `pandas`, `numpy`, `matplotlib`, `openpyxl`, `pdfplumber`

Install dependencies using:
```bash
pip install -r requirements.txt
```

## Results

The analysis reveals potential differences between officially reported and manually calculated AQI values. These discrepancies could result from different calculation methodologies, missing data, or rounding differences.

## Contributing

Contributions are welcome! If you find any issues or have suggestions, feel free to create a pull request or open an issue.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
