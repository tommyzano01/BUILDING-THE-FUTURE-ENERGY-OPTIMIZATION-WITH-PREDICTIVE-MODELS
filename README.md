# BUILDING-THE-FUTURE-ENERGY-OPTIMIZATION-WITH-PREDICTIVE-MODELS

This project presents a predictive model based on an Artificial Neural Network (ANN) to estimate the heating load of residential buildings using eight geometric and design-related parameters.  
Trained with JAX and optimized using the Adam algorithm, the model was validated through statistical analysis, Monte Carlo simulations, and an interactive user interface.

---

## Project Summary

- **Dataset**: `DATASET.xlsx`  
- **Model**: Artificial Neural Network (ANN)  
- **Framework**: JAX (training and optimization)  
- **Optimization**: Adam algorithm  
- **Extra techniques**: Feature Importance + Monte Carlo simulation  
- **Tool**: Simple and interactive, suitable for non-experts  

---

## Files

- `Project_GR09.ipynb` – Main notebook with full model code and analysis.  
- `DATASET.xlsx` – Required input data to run the model.  

---

## How to Use in Google Colab

1. Download both files from the repository:
   - `Project_GR09.ipynb`
   - `DATASET.xlsx`

2. Open [Google Colab](https://colab.research.google.com/) and click **"File" > "Upload notebook"** to upload the `.ipynb` file.

3. When running the **first code block**, you will be prompted to upload the Excel file. Wait for the file upload prompt, then:

   - Click the "Choose Files" button
   - Select and upload the `DATASET.xlsx` file

   The upload is handled by the following code in the notebook:

   ```python
   from google.colab import files
   uploaded = files.upload()

   import pandas as pd
   df = pd.read_excel("DATASET.xlsx")
   df.head()
