# BUILDING-THE-FUTURE-ENERGY-OPTIMIZATION-WITH-PREDICTIVE-MODELS

This work presents a predictive model based on an Artificial Neural Network (ANN) to estimate the heating load of residential buildings using eight geometric and design-related parameters.  
Trained with JAX and optimized using the Adam algorithm, the model was validated through statistical analysis, Monte Carlo simulations, and an interactive user interface.

---

## Project Summary

- **Dataset**: `DATASET.xlsx`
- **Model**: Artificial Neural Network (ANN)
- ⚙**Framework**: JAX (training and optimization)
- **Optimization**: Adam algorithm
- **Extra techniques**: Feature Importance + Monte Carlo simulation
- **Interface**: Simple and interactive, suitable for non-experts

---

## Files

- `Managment_GR09_def (1).ipynb` – Main notebook with full model code and analysis.
- `DATASET.xlsx` – Required input data to run the model.

---

## How to Use in Google Colab

1. Open the notebook in Google Colab.
2. Upload both the `.ipynb` file and the `DATASET.xlsx` file to the Colab session.
3. The dataset must be uploaded **after the following block of code**, which allows file selection:

```python
from google.colab import files
uploaded = files.upload()

import pandas as pd
df = pd.read_excel("DATASET.xlsx")
df.head()
