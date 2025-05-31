# Sleep Event Prediction from Accelerometer Data

**Course:** CS 184A/284A – AI in Biology and Medicine
**Contributors:** Diya Saha ([sahad1@uci.edu](mailto:sahad1@uci.edu)), Abhinand Ganesh ([aganesh5@uci.edu](mailto:aganesh5@uci.edu))

## Project Overview

This project aims to predict **sleep onset** and **wake-up events** using accelerometer data collected from wearable devices. The task is framed as a **time series event detection** or **sequence labeling** problem. By leveraging a combination of classical time series analysis techniques and modern deep learning models, we developed an efficient and interpretable pipeline for detecting sleep events in real-world data from multiple subjects.

## Dataset

Due to GitHub storage limitations, we provide example datasets for the following `series_id` values:

* `1b92be89db4c`
* `655f19eabf1e`
* `5c55a5e717d6`

### Available Data Files

* `data/train_events_csv.csv` – Contains labeled sleep onset and wake-up events.
* `data/pandas_df.csv` – Contains time series accelerometer data for the selected subjects.

## Requirements

Install the following Python libraries before running the code:

```bash
pip install tensorflow pandas numpy matplotlib scikit-learn
```

## Getting Started

### Step 1: Load the Datasets

```python
import pandas as pd

train_events_csv = pd.read_csv('data/train_events_csv.csv')
pandas_df = pd.read_csv('data/pandas_df.csv')
```

### Step 2: Run Feature Expansion

```python
random_series = ['1b92be89db4c', '655f19eabf1e', '5c55a5e717d6']
feature_df = merging_patients(random_series)
```

## Methodology

* **Data Preprocessing:** Normalization, feature extraction, and windowing of time series data.
* **Modeling:** Implemented traditional time series methods and deep learning architectures to detect events.
* **Evaluation:** Measured prediction accuracy, precision, and recall for sleep onset and wake-up events.

## Results

Our model performed reliably across sampled subjects, detecting sleep events with a balance of sensitivity and specificity. Future work includes expanding to larger datasets and optimizing for real-time inference.

## License

This project is for academic use only and was developed as part of a UC Irvine course project.
