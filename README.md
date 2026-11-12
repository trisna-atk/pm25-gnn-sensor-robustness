# Evaluating GraphSAGE Robustness under Random and Spatially Localized Sensor Failures for Urban PM2.5 Prediction

## Research Overview

This repository contains the implementation and experimental documentation for evaluating the robustness of GraphSAGE, Graph Convolutional Network (GCN), and Graph Attention Network (GAT) models for urban PM2.5 prediction.

The experiments use the Beijing Multi-Site Air Quality dataset, which consists of 12 air quality monitoring stations.

The study evaluates model performance under three conditions:
- Normal condition (0% sensor failure).
- Random sensor failure.
- Spatially localized sensor failure.

## Research Objectives

The objectives of this research are:
1. To evaluate the baseline performance of GraphSAGE, GCN, and GAT.
2. To investigate the effects of random sensor failures on PM2.5 prediction.
3. To investigate the effects of spatially localized sensor failures.
4. To compare model robustness at different sensor failure levels.

## Dataset

Dataset: Beijing Multi-Site Air Quality

Source: UCI Machine Learning Repository  
https://archive.ics.uci.edu/dataset/501/beijing+multi+site+air+quality+data

The dataset contains air pollutant measurements and meteorological variables collected from 12 monitoring stations in Beijing.

## Experimental Setup

**Models:**
- GraphSAGE
- Graph Convolutional Network (GCN)
- Graph Attention Network (GAT)

**Sensor Failure Levels:**
- 0% (normal condition)
- 8.33%
- 25%
- 50%
- 75%

**Failure Scenarios:**
- Random sensor failure
- Spatially localized sensor failure

**Evaluation Metrics:**
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Coefficient of Determination (R²)
- MAE Degradation (%)

## Repository Structure

```text
pm25-gnn-sensor-robustness/
├── README.md
├── requirements.txt
├── .gitignore
├── data/
├── notebooks/
├── src/
├── results/
└── figures/
```

## Installation

Create a Python virtual environment:

```bash
python -m venv .venv
```

Install the required packages:

```bash
pip install -r requirements.txt
```

PyTorch and PyTorch Geometric installation may depend on the operating system and CPU/CUDA configuration. Refer to their official installation guides.

## Reproducibility

To reproduce the experiments:

1. Clone this repository.
2. Install the required dependencies.
3. Download the dataset from the UCI repository.
4. Follow the data preparation instructions.
5. Run the notebooks in the specified order.
6. Execute model training and sensor failure simulations.
7. Evaluate the models using MAE, RMSE, R², and MAE degradation.

The experiments use a random seed of 42.

## Results

Experimental results and visualizations will be provided in the `results/` and `figures/` directories.

## Research Contribution

This research provides a comparative evaluation of GraphSAGE, GCN, and GAT under random and spatially localized sensor failure scenarios. The study focuses on understanding how different sensor failure patterns and failure levels affect the predictive performance and robustness of graph neural network architectures.

## Citation

Citation information will be added after publication of the research paper.
