# Data Sourcing Challenge

The goal of this challenge is to retrieve, process, and merge data from multiple sources (Coronal Mass Ejections (CME) and Geomagnetic Storms (GST) data from the NASA API), showcasing data engineering skills and preparing the data for analysis.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Setup and Requirements](#setup-and-requirements)
- [Usage](#usage)
- [Data Sources](#data-sources)
- [Output](#output)

---

## Overview
This project retrieves CME and GST data from the NASA DONKI API (https://api.nasa.gov/DONKI/), processes the retrieved data, and merges it into a single dataset for further analysis. The workflow includes:

1. Fetching data from the NASA DONKI API.
2. Cleaning and processing the retrieved data.
3. Merging the datasets into a single cohesive file.
4. Exporting the final dataset as a CSV file.

---

## Features
- **Data Retrieval**: Extracts data from the NASA DONKI API.
- **Data Cleaning**: Handles missing values and standardizes columns.
- **Data Merging**: Combines the datasets into a single dataset.
- **Output Export**: Saves the final merged dataset to a CSV file.

---

## Setup and Requirements

### Prerequisites
To run the analysis, ensure you have:
- **Python**: Version 3.10 or later.
- **Jupyter Notebook** or **JupyterLab**.
- The following Python library:
  - `pandas`

Install required libraries using:
```bash
pip install pandas
```

### Environment Variables
The project uses environment variables to securely store API keys. Add the following to a `.env` file in the root directory:

```
NASA_API_KEY=your_nasa_api_key_here
```

---

## Usage

1. Clone the repository:
```bash
git clone https://github.com/jesseparent/data-sourcing-challenge.git
cd data-sourcing-challenge
```

2. Ensure the `.env` file is properly set up with a valid NASA API key.

3. Run the Jupyter Notebook to execute the data retrieval and merging process:
```bash
jupyter notebook retrieve_data.ipynb
```

4. The output CSV file will be saved as `merged_gst_cme.csv` in the root directory.

---

## Data Sources
- **NASA DONKI API**: Provides information about solar events such as coronal mass ejections, solar flares, and geomagnetic storms.

---

## Output
- The final dataset (`merged_gst_cme.csv`) includes the merged data from the two data sources, as well as a time_diff that shows the difference in time from when a CME occurs to when a GST occurs.

---


