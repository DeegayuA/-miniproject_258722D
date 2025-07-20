# Climate Anomaly Detection in Sri Lanka using Isolation Forest

> 📚 **Course:** CS5803 – Advanced Data Mining  
> 👤 **Author:** Deeghayu Adhikari  
> 🆔 **Project ID:** `258722D`  
> 🎓 Master of Data Science and AI, CSE, University of Moratuwa

---

## 1. Project Overview

This project conducts a data-driven analysis of climate anomalies in Sri Lanka using a comprehensive weather dataset spanning from **January 2010 to June 2023**. The goal is to identify statistically significant deviations from normal weather patterns, which can serve as key indicators of climate instability and the local impacts of climate change.

The core methodology involves:
1.  **Data Preprocessing:** Cleaning and preparing the dataset of over 147,000 records.
2.  **Exploratory Data Analysis (EDA):** Visualizing distributions and trends to understand underlying meteorological patterns.
3.  **Feature Engineering:** Creating time-aware features, such as 7-day rolling temperature averages, to improve model context.
4.  **Anomaly Detection:** Applying an **Isolation Forest** algorithm to detect unusual weather events based on 14 key features like temperature, precipitation, and wind.
5.  **Analysis & Visualization:** Interpreting the detected anomalies by examining their geographical and temporal distributions and visualizing them on time-series plots.

---

## 2. Key Insights & Findings

The analysis successfully uncovered significant patterns of climate instability. Key insights include:

*   **Significant Volatility Detected:** The Isolation Forest model identified **20,065 anomalous days** (~13.6% of the dataset), indicating that unusual weather events are a notable feature of Sri Lanka's climate over the past decade.

*   **Geographical Concentration of Anomalies:** The anomalies are not uniformly distributed. The cities most affected are concentrated in the central highlands and specific coastal regions:
    1.  **Hatton:** 4,913 anomalies
    2.  **Badulla:** 2,528 anomalies
    3.  **Kandy:** 1,847 anomalies

*   **Temporal Hotspots:** Certain years experienced a higher frequency of anomalies, with **2014, 2010, and 2016** standing out as the most volatile years in the dataset.

*   **The "Anomaly Profile":** Anomalous days are defined by extreme conditions, especially:
    *   **Extreme Precipitation:** On average, anomalous days recorded nearly **3 times more rainfall** than normal days.
    *   **High Temperature Variance:** While the mean temperature was slightly lower on anomalous days, the standard deviation was much higher, pointing to more extreme temperature swings (both hotter highs and colder lows).
    *   **Common Weather Events:** Anomalies were most frequently associated with moderate rain (`weathercode` 63), drizzle (51), and surprisingly, clear skies (1), suggesting unusual heat or cold snaps.

---

## 3. Repository Structure

This repository is organized as follows:

<pre><code>
```
miniproject_258722D/
│
├── data/
│   └── SriLanka_Weather_Dataset.csv         # The raw dataset used for analysis.
│
├── notebooks/
│   └── Project_Data_mining_Deeghayu.ipynb   # Jupyter Notebook containing the complete analysis.
│
├── requirements.txt                         # Python dependencies for the project.
└── README.md                                # This file.
```
</code></pre>


## 4. How to Run the Project

This project was developed using Python 3. The entire analysis is encapsulated within the provided Jupyter Notebook.

### Prerequisites

-   Python 3.8+
-   `pip` package manager
-   A virtual environment tool (`venv` or `conda`) is strongly recommended.

### Setup Instructions

1.  **Clone the Repository:**
    ```sh
    git clone https://github.com/your-username/miniproject_258722D.git
    cd miniproject_258722D
    ```

2.  **Create and Activate a Virtual Environment:**
    ```sh
    # Using venv
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install Dependencies:**
    The `requirements.txt` file lists all necessary libraries. Install them using pip:
    ```sh
    pip install -r requirements.txt
    ```

### Execution

1.  **Start Jupyter:**
    ```sh
    jupyter lab  # or jupyter notebook
    ```

2.  **Open the Notebook:**
    Navigate to the `notebooks/` directory and open `Project_Data_mining_Deeghayu.ipynb`.

3.  **Run All Cells:**
    To reproduce the analysis and all outputs, select **"Run" > "Run All Cells"** from the menu.

### Expected Runtime and Software Versions

-   **Expected Runtime:** The entire notebook should execute in **under 2 minutes** on a standard modern laptop.
-   **Key Software Versions:**
    -   `pandas==1.5.3`
    -   `scikit-learn==1.2.2`
    -   `matplotlib==3.7.1`
    -   `seaborn==0.12.2`

