# Traffic Flow Anomaly Detection

Detect anomalies in network traffic using the Isolation Forest algorithm. The Streamlit app provides interactive visualizations, dataset stats, and export options.

## Live App

https://traffic-flow-anomaly.streamlit.app/

## Screenshot
<img width="2877" height="1625" alt="image" src="https://github.com/user-attachments/assets/9ead81e2-0e89-4b0f-8190-26b8fc846e28" />

## Features

- Upload a CSV file or use the sample dataset
- Adjustable contamination rate and number of trees
- 2D and 3D anomaly visualizations
- Summary statistics and feature variance analysis
- Export results and reports

## Project Structure

- app.py: Streamlit application
- embedded_system_network_security_dataset.csv: Sample dataset
- isolation_forest_model.pkl: Trained model artifact
- network_anomaly.ipynb: Exploration notebook

## Requirements

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run Locally

```bash
streamlit run app.py
```

## Notes

- The app drops a column named `label` if present in the dataset.
- Boolean columns are converted to integers and missing values are filled with the column mean.
