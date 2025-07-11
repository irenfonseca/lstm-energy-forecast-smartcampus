# LSTM-Based Energy Forecasting Dataset – Smart Campus UA

This repository provides a public dataset and baseline configuration files used in the study:

**"From Comparison to Deployment: Operationalizing LSTM Energy Forecasting for Smart Campuses"**

The dataset contains hourly electricity consumption records from a university building over a two-year period (2019–2020), used to train and evaluate LSTM-based forecasting models in a smart campus environment.

---

## 📁 Dataset

**Filename:** `smartcampus_energy_buildingA_ua_2019_2020.csv`  
**Format:** CSV (UTF-8)  
**Size:** ~17,500 rows × 6 columns  
**Granularity:** Hourly (1-hour intervals)  
**Location:** University of Alicante (Spain)

### Columns

| Column Name        | Description                                       |
|--------------------|---------------------------------------------------|
| `consumption_kwh`  | Energy consumption in kilowatt-hours (float)      |
| `hour`             | Hour of day (0–23)                                |
| `day_of_week`      | Day of week (0=Monday, 6=Sunday)                  |
| `day_of_month`     | Calendar day (1–31)                               |
| `month`            | Month (1–12)                                      |

> Contextual variables (hour, day, etc.) are included to support time-aware model training.

---

## 📌 Use Case

This dataset was used to train and evaluate three LSTM configurations:
- **Model A:** Full context (consumption + calendar features)
- **Model B:** Minimalist (only consumption)
- **Model C:** PCA-reduced context

It supports reproducible experimentation in energy forecasting, edge AI deployment, and smart campus research.

---

## 📜 License

This dataset is published under the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/).  
You are free to use, share, and adapt the data with appropriate attribution.

---

## 📚 Citation

If you use this dataset in your research, please cite:

> [Authors]. *From Comparison to Deployment: Operationalizing LSTM Energy Forecasting for Smart Campuses*. Submitted to Applied Soft Computing, 2025.

And reference the dataset DOI (to be assigned by Zenodo).

---

## 🔗 Related Resources
- Paper DOI (pending)
- Model training code (optional)


