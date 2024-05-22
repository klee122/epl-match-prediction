# EPL Match Prediction

This Jupyter Notebook provides a framework for predicting English Premier League (EPL) match outcomes using various models based on mathematical modelling on football team's past performances. It includes functions for calculating goal expectancies, plotting heat maps, and visualizing predictions using Poisson distribution graphs.

## Overview

The notebook consists of the following main components:
1. **Data Preparation**
2. **Modeling**
3. **Visualization**

### Data Preparation
- **Teams and Statistics**: The notebook includes sample data for EPL teams and their statistical attributes such as attack strength, defense strength, average goals, and possession strength.
- **Data Files**: The data is provided in the following files:
  - `EPL Analysis.xlsx`
  - `Strengths.xlsx`

### Modeling
- **Goal Expectancy Calculation**: Functions to compute home and away goal expectancies based on different models (`m1`, `m2`, `m3`, and `m4`).
- **Model Class**: A Python class `Model` is defined to encapsulate the goal expectancies and model name.

### Visualization
- **Heat Maps**: The `PlotHeatMap` function generates a heat map showing the probability distribution of match outcomes (home goals vs. away goals).
- **Poisson Graphs**: The `PlotPoissonGraph` visualizes predictions using Poisson distribution graphs.

## Usage

### 1. Data Setup
Ensure you have the provided data files (`EPL Analysis.xlsx` and `Strengths.xlsx`) in the same directory as the notebook. The notebook will read these files to load the necessary statistics for EPL teams.

### 2. Predicting Match Outcomes
Use the `PredictResult` function to predict the outcome of a match between two teams:

```python
PredictResult("Team A", "Team B", "m1")
```
### 3. Plotting Heat Maps

The `PlotHeatMap` function visualizes the distribution of match outcomes as a heat map. It is automatically called within the `PredictResult` function.

## Requirements

* Python 3.x
* Jupyter Notebook
* Pandas
* Matplotlib
* NumPy
* Openpyxl (for reading Excel files)

### Installation

```bash
pip install pandas matplotlib numpy jupyter openpyxl
```

### Running the Notebook

1. Clone the repository or download the notebook file.
2. Ensure the `EPL Analysis.xlsx` and `Strengths.xlsx` files are in the same directory as the notebook.
3. Navigate to the directory containing the notebook.
4. Start Jupyter Notebook:

    ```bash
    jupyter notebook
    ```

5. Open the `epl-prediction.ipynb` notebook and run the cells.
