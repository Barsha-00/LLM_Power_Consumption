# Energy Disaggregation using LLaMA-3.3-70B via Groq API

## Author
**Barsha Sadhu**

## Overview

Using a preprocessed dataset taken from the "Individual household electric power consumption" dataset, this project carries out energy disaggregation (also known as non-intrusive load monitoring, or NILM). Utilising the llama-3.3-70b-versatile model through the Groq API platform, the project leverages the power of large language models (LLMs) to address a variety of insightful dataset queries.

## Groq API and LLM Used

- **LLM**: `llama-3.3-70b-versatile`
- **API Platform**: [Groq API Console](https://console.groq.com)
- **Purpose**: Natural language-driven data querying and script generation for power consumption analytics.

## Dataset

- **Source**: UCI Machine Learning Repository
- **File Used**: `household_power_consumption.csv`
- **Size**: ~2M entries, sampled at 1-minute intervals

## Summary of Tasks Completed

1. **Data Preprocessing**
  - Combined `Date` and `Time` columns into a single `datetime` index
  - Handled missing values and type conversion
  - Filtered relevant timeframes and columns for targeted analysis
  - 
2. **Natural Language Queries to LLM**
   - Asked intelligent questions to the LLM model.

3. **LLM-Based Code Generation**
   - Used Groq API to generate Python scripts on-the-fly based on each query
   - Ran and verified the generated code for correctness and insight

4. **Visualization and Statistical Analysis**
   - Created bar charts, line plots, and correlation heatmaps
   - Interpreted seasonal and daily energy usage trends



