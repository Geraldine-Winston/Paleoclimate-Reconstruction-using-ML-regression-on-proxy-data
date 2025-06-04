# Paleoclimate Reconstruction using ML Regression on Proxy Data

This project applies **Machine Learning regression models** to reconstruct past climate conditions, specifically **paleotemperatures**, using proxy data such as isotope ratios, pollen counts, and sediment properties.

## Project Overview

- **Input**: Proxy data including isotope ratios, pollen indices, sediment density, and magnetic susceptibility.
- **Target**: Reconstruct past temperature values.
- **Model**: Random Forest Regressor trained to predict paleotemperatures from proxy data.
- **Output**: Predicted past temperatures based on given proxy measurements.

## Project Structure

```
📁 Paleoclimate-Reconstruction-ML
├── proxy_climate_data.xlsx        # Synthetic proxy climate dataset
├── paleoclimate_rf_model.pkl      # Trained Random Forest model
├── paleoclimate_reconstruction.py # Main training and evaluation script
├── README.md                      # Project documentation
├── requirements.txt               # Python dependencies
└── .gitignore                      # Files to ignore in version control
```

## Requirements

Install all necessary dependencies using:

```bash
pip install -r requirements.txt
```

**Dependencies:**

```
pandas
numpy
scikit-learn
openpyxl
joblib
```

## How to Run

1. Ensure `proxy_climate_data.xlsx` is available in your project directory.
2. Run the script:

```bash
python paleoclimate_reconstruction.py
```

3. After training:
   - Model evaluation metrics (MSE and R² Score) will be printed.
   - The trained model will be saved as `paleoclimate_rf_model.pkl`.

## Dataset Example

```csv
Isotope_Ratio,Pollen_Index,Sediment_Density,Magnetic_Susceptibility,Temperature
-1.56,45.2,2.65,800,13.7
2.33,60.1,2.55,600,14.5
...
```

## Model Performance

The Random Forest model achieves:
- **Test MSE**: ~1.02
- **Test R² Score**: ~0.91

*(Values may vary depending on data and random seed.)*

## Acknowledgements

- Inspired by real-world paleoclimate reconstruction studies.
- Future extensions could involve more complex models and the use of real-world datasets from the **NOAA Paleoclimatology Database** or **PANGAEA**.

## Author

**Ayebawanaemi Geraldine Winston**

