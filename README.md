# Assignment 1: Data Profiling (EDA) Report

**Course:** TTTC3213  
**Domain:** Finance / FinTech  
**Dataset:** UCI Statlog (German Credit Data)

This assignment evaluates data quality through missing-information checks, duplicate detection, numerical and categorical validation, outlier flagging, diagnostic charts, and privacy and bias assessment. Team members and matric numbers are listed in the notebook.

## Files

- `Assignment1_Data_Profiling.ipynb`: Main report, executable analysis, and saved outputs.
- `assignment1_data_profiling.py`: Python export of the revised notebook.
- `README.md`: Data source and run instructions.

## Data source

[UCI Statlog (German Credit Data)](https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data)

The notebook downloads the public ZIP archive, extracts it, and loads `german.data`. The dataset contains 1,000 records, 20 predictors, and one credit-risk target.

Citation: Hofmann, H. (1994). *Statlog (German Credit Data).* UCI Machine Learning Repository. https://doi.org/10.24432/C5NC77

## Run in Google Colab

[Open the notebook in Colab](https://colab.research.google.com/github/HaziqSyakir/Assignment1-Data-Profiling/blob/main/Assignment1_Data_Profiling.ipynb)

1. Open the notebook.
2. Connect to a Python runtime with internet access.
3. Restart the session and run all cells from top to bottom.
4. Review the generated tables, charts, handling log, and conclusion.

No manual dataset upload is required. Files are downloaded into `data/german_credit` under the runtime’s working directory.

## Run locally

Use a Python environment with pandas, NumPy, Matplotlib, seaborn, IPython, and Jupyter Notebook installed:

```bash
python -m pip install pandas numpy matplotlib seaborn ipython notebook
```

Open `Assignment1_Data_Profiling.ipynb` in Jupyter and run all cells from top to bottom. Internet access is required for the dataset download.

The Python export can also be run with:

```bash
python assignment1_data_profiling.py
```

## Interpretation

The workflow preserves all original records and values and adds three numerical-outlier flags. Ambiguous categories and remaining limitations are documented in the notebook. Passing the implemented checks does not establish readiness for operational lending decisions.