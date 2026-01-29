# Quantitative Analysis of Social Movement Dynamics

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Millrjess/Jess/blob/main/protest_analysis_FINAL_VERSION.ipynb)
[![View in NBViewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/Millrjess/Jess/blob/main/protest_analysis_FINAL_VERSION.ipynb)

## 📊 Project Overview
This project investigates the driving forces behind social protest frequency using a dataset of global events. I developed a robust statistical framework to determine how population density and temporal shifts impact the scale of social mobilization.

## 🧠 Statistical Methodology: Why Negative Binomial?
In social science data, event counts often exhibit **overdispersion**, where the variance significantly exceeds the mean. A standard Poisson model assumes these values are equal; ignoring overdispersion leads to underestimated standard errors and "false" significance.



By estimating the dispersion parameter (**alpha**) at **0.7573** ($p < 0.001$), this analysis confirms that a **Negative Binomial Generalized Linear Model (GLM)** is the statistically appropriate choice, ensuring the reliability of the findings.

## 📈 Key Findings
* **Population Density (LOG_POP):** Identified as the strongest predictor of activity ($\beta = 0.4561$). This confirms the "Critical Mass" theory, where higher population density reduces the organizational costs of mobilization.
* **Temporal Trends (CENTERED_YEAR):** Holding population constant, the model identified a statistically significant annual decline in protest frequency ($\beta = -0.1440$).
* **Model Robustness:** The model achieved an Log-Likelihood Ratio (LLR) p-value of **1.025e-28**, indicating the results are highly robust and statistically significant.



## 🛠️ Tech Stack
* **Language:** Python 3.10+
* **Modeling:** `statsmodels` (Negative Binomial GLM)
* **Data Handling:** `pandas`, `numpy`
* **Visualization:** `matplotlib` (Refactored for publication-ready styling)

## 🚀 How to View & Run
1.  **Instant View:** Use the [NBViewer link](https://nbviewer.org/github/Millrjess/Jess/blob/main/protest_analysis_FINAL_VERSION.ipynb) for a fast, high-quality rendering of the LaTeX math and plots.
2.  **Interactive Execution:** Click the **Google Colab badge** at the top to run the analysis live in your browser.
3.  **Local Environment:**
    ```bash
    git clone [https://github.com/Millrjess/Jess.git](https://github.com/Millrjess/Jess.git)
    pip install pandas statsmodels matplotlib
    ```

## 📝 Conclusion
The analysis demonstrates that urbanization and population exposure are the primary structural drivers of social movements. The methodology used here provides a scalable framework for predicting "mobilization hot zones" across different geopolitical cycles.

---
*Analysis by Jess — Data Science Portfolio Piece*
