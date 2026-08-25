# Freight Rate Prediction Challenge

This repository contains the implementation for the freight rate prediction model.

## Run Instructions

### Prerequisites
- **Python**: Installed and configured on your system.
- **Environment**: A Jupyter Notebook environment (e.g., VS Code, JupyterLab).
- **Data**: The required dataset files must be placed in the `data/` directory before execution. *Note: Data is excluded from this repository to prevent leakage of assessment materials.*

### Execution
1. Open `Spotter.ai Assessment.ipynb`.
2. **Run the cells sequentially (one by one)** from top to bottom.
3. All necessary dependencies are installed automatically via the first cell of the notebook.

## Project Components
- `Spotter.ai Assessment.ipynb`: End-to-end pipeline including data cleaning, feature engineering (cyclic date features), model training (MLPRegressor), and prediction.
- `score.py`: Scorer script to validate output.
- `requirements.txt`: Dependency list.
- `validation_predictions.csv`: Final predictions for the validation set.

## Validation
After executing the notebook, the predictions can be scored using:

```bash
python score.py --predictions validation_predictions.csv --december-predictions data/december_chart_inputs.csv
