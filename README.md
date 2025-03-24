# Integrated-Energy-System-Multi-Load-Anomaly-Detection

# Energy Load Analysis and Clustering

This project focuses on analyzing energy load data, decomposing signals using Variational Mode Decomposition (VMD), and performing clustering and anomaly detection.

## Requirements
Ensure you have the required dependencies installed:
```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels sklearn vmdpy
```

## Data Preprocessing
- Load energy data from `energy_data.xlsx`
- Perform unit conversions for `CHWTON` and `HTmmBTU`
- Remove redundant features
- Compute correlation heatmap
- Select influencing features for prediction

## Variational Mode Decomposition (VMD)
- Compute Mean Squared Reconstruction Error (MSRE) for different values of `K`
- Perform VMD on electric, heating, and cooling loads
- Extract high-frequency Intrinsic Mode Functions (IMFs)

## Clustering
- KMeans clustering on VMD-transformed features
- PCA visualization of clusters
- Hierarchical clustering with anomaly detection

## Anomaly Detection
- Hierarchical clustering-based anomaly detection
- Singular Value Decomposition (SVD) for anomaly detection
- Comparison of anomaly detection techniques

## Visualization
- Correlation heatmap
- MSRE vs. `K` plots
- Cluster visualizations using PCA
- Anomaly detection results comparison

## Running the Analysis
Run the Python script to process the data, perform VMD, clustering, and anomaly detection:
```bash
python energy_analysis.py
```

## Output
The script generates:
- Processed datasets with selected features
- VMD decomposed signals
- Clustered datasets with visualizations
- Anomaly detection results

## Authors
Developed by Hao Ru.
