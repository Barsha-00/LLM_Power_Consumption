# Energy Disaggregation using LLaMA-3.3-70B via Groq API

## Author
**Barsha Sadhu**

## Overview

This project focuses on non-intrusive energy disaggregation using a publicly available household energy dataset. The analysis leverages a large language model (LLM), **LLaMA-3.3-70B-Versatile**, accessed through the **Groq API**, to dynamically generate Python scripts that answer specific analytical queries on the dataset.

## Groq API and LLM Used

- **LLM**: `llama-3.3-70b-versatile`
- **API Platform**: [Groq API Console](https://console.groq.com)
- **Purpose**: Natural language-driven data querying and script generation for power consumption analytics.

## Dataset

- **Name**: Individual Household Electric Power Consumption Dataset
- **Format**: CSV
- **File Used**: `household_power_consumption (1).csv`
- **Preprocessing Includes**:
  - Combined `Date` and `Time` columns into a single `DateTime` index
  - Removed missing values and converted types
  - Filtered relevant timeframes and columns for targeted analysis

## Summary of Tasks Completed

1. **Data Preprocessing**
   - Cleaned and formatted the raw dataset
   - Resampled and transformed power readings for specific use cases

2. **Natural Language Queries to LLM**
   - Asked intelligent questions like:
     - What was the average energy usage in March 2007?
     - What hour on Christmas 2006 had the highest usage?
     - Compare weekday vs weekend usage
     - Plot energy usage for specific periods
     - Compute correlation between power and sub-metering data

3. **LLM-Based Code Generation**
   - Used Groq API to generate Python scripts on-the-fly based on each query
   - Ran and verified the generated code for correctness and insight

4. **Visualization and Statistical Analysis**
   - Created bar charts, line plots, and correlation heatmaps
   - Interpreted seasonal and daily energy usage trends

## Helper Scripts (Optional/Recommended)

If separating concerns in your repo:

- `preprocess_data.py` — For converting and cleaning the raw dataset
- `query_llm.py` — Script to interact with the Groq API and generate code
- `visualize.py` — For all Matplotlib/Seaborn plots
- `requirements.txt` — Python dependencies (`pandas`, `matplotlib`, `seaborn`, `groq`)

## Example Usage

```bash
python preprocess_data.py   # Prepares dataset
python query_llm.py         # Asks LLM to generate analysis code

