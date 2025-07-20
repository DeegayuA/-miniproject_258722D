# Climate Anomaly Detection in Sri Lanka using Isolation Forest

> 📚 **Course:** CS5803 – Advanced Data Mining  
> 👤 **Author:** Deeghayu Adhikari  
> 🆔 **Project ID:** `258722D`  
> 🎓 Master of Data Science and AI, CSE, University of Moratuwa

---

---

## 1. Project Overview

This project conducts a data-driven analysis of climate anomalies in Sri Lanka using a weather dataset spanning from 2010 to 2023. The goal is to identify statistically significant deviations from normal weather patterns, which may serve as indicators of climate instability.

The core methodology involves:
1.  **Data Preprocessing:** Cleaning and preparing the dataset for time-series analysis.
2.  **Exploratory Data Analysis (EDA):** Understanding the distributions and trends of key meteorological variables.
3.  **Feature Engineering:** Creating time-aware features like rolling averages and lagged variables to enhance model performance.
4.  **Anomaly Detection:** Applying an **Isolation Forest** model to detect unusual weather events based on a multi-feature input.
5.  **Analysis & Visualization:** Interpreting the detected anomalies by examining their geographical and temporal distributions and visualizing them on time-series plots.

The analysis successfully identified over 20,000 anomalous days, with notable concentrations in specific cities (e.g., Hatton, Badulla) and years.

## 2. Repository Structure

This repository is organized as follows:
miniproject_<your-id>/
│
├── data/
│ ├── SriLanka_Weather_Dataset.csv # The raw dataset used for analysis
│ └── (or a script to download the data if it's too large)
│
├── notebooks/
│ └── Project_Data_mining_Deeghayu (1).ipynb # Jupyter Notebook with the full analysis
│
├── src/
│ └── (Optional: Any helper scripts or Python modules if the code is refactored)
│
├── requirements.txt # Python dependencies for the project
└── README.md # This file

## 3. How to Run the Project

This project was developed using Python 3 and standard data science libraries. The analysis is contained within a single Jupyter Notebook.

### Prerequisites

-   Python 3.8+
-   `pip` package manager
-   A virtual environment tool (`venv` or `conda`) is highly recommended.

### Setup Instructions

1.  **Clone the repository:**
    ```sh
    git clone <repository-url>
    cd miniproject_<your-id>
    ```

2.  **Create and activate a virtual environment:**
    ```sh
    # Using venv
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

    # Or using Conda
    # conda create -n datamining_env python=3.8
    # conda activate datamining_env
    ```

3.  **Install the required dependencies:**
    The `requirements.txt` file lists all necessary libraries. Install them using pip:
    ```sh
    pip install -r requirements.txt
    ```

### Execution

1.  **Start Jupyter Lab or Jupyter Notebook:**
    ```sh
    jupyter lab
    ```
    or
    ```sh
    jupyter notebook
    ```

2.  **Open the notebook:**
    Navigate to the `notebooks/` directory and open `Project_Data_mining_Deeghayu (1).ipynb`.

3.  **Run the cells:**
    Execute the cells sequentially from top to bottom. All figures and tables will be generated directly within the notebook.

### Expected Runtime and Software Versions

-   **Expected Runtime:** The entire notebook should execute in **under 2 minutes** on a standard modern laptop.
-   **Key Software Versions:**
    -   `pandas==<version_from_your_env>` (e.g., 1.5.3)
    -   `scikit-learn==<version_from_your_env>` (e.g., 1.2.2)
    -   `matplotlib==<version_from_your_env>` (e.g., 3.7.1)
    -   `seaborn==<version_from_your_env>` (e.g., 0.12.2)
    -   `jupyterlab==<version_from_your_env>` (e.g., 3.6.3)

*(**Note to user:** Replace `<your-id>` and `<version_from_your_env>` with your actual details. You can generate the exact versions for `requirements.txt` by running `pip freeze > requirements.txt` in your activated virtual environment.)*

---
