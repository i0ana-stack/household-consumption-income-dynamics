\# Household Consumption and Income Dynamics



\## Project Overview



This project analyzes the relationship between household consumption, real personal income, prices, economic activity, and employment across U.S. states using panel data.



The analysis covers \*\*2008–2024\*\* and applies several panel-data econometric approaches, including Fixed Effects, Random Effects, log-linear specifications, dynamic analysis, robustness checks, and a Hausman test.



The project was developed as part of my Master's research in \*\*Data Analysis in Business\*\*.



\## Research Objective



The main objective is to examine how changes in real personal income are associated with household consumption across U.S. states over time, while accounting for state-specific and year-specific effects.



The analysis also investigates how the estimated relationship changes under different model specifications and variable scaling approaches.



\## Dataset



The analysis uses annual panel data for \*\*52 U.S. entities\*\* over the \*\*2008–2024\*\* period, resulting in \*\*884 observations\*\*.



The dataset includes measures of:



\- Personal Consumption Expenditure (PCE)

\- Real Personal Income

\- Regional Price Parities (RPPs)

\- Real Gross Domestic Product

\- Employment

\- Personal Income

\- Personal Income Per Capita

\- Real Personal Income Per Capita



\## Methodology



The project applies several econometric specifications to examine the relationship between real personal income and consumption:



\- Fixed Effects (FE)

\- Random Effects (RE)

\- Log-linear Fixed Effects

\- Dynamic Fixed Effects

\- Per-worker robustness specification

\- Hausman specification test

\- Descriptive statistics and correlation analysis



State and year fixed effects are used in the main Fixed Effects specifications to account for unobserved differences across entities and common changes over time.



\## Key Findings



The analysis produces several main findings:



\- The main log-linear Fixed Effects model estimates an income-consumption elasticity of \*\*0.6867\*\*. A 1% increase in real personal income is associated with approximately a 0.69% increase in personal consumption expenditure, holding entity and year effects fixed.

\- Consumption shows strong persistence over time. In the dynamic Fixed Effects model, the lagged consumption coefficient is approximately \*\*0.7894\*\*, while the real personal income coefficient falls to \*\*0.1963\*\*.

\- The per-worker robustness specification estimates an elasticity of \*\*0.3203\*\*, indicating that the positive association remains after scaling the aggregate variables by employment.

\- The Random Effects model estimates a substantially larger elasticity of \*\*0.9827\*\*. The Hausman test rejects the null hypothesis with a p-value below 0.001, supporting Fixed Effects over Random Effects for the main log-linear comparison.

\- Several aggregate economic variables are extremely highly correlated. For example, Real Personal Income and Real GDP have a correlation of \*\*0.9991\*\*, while Real Personal Income and Employment have a correlation of \*\*0.9975\*\*.

\- The estimated income coefficient changes considerably across specifications, highlighting the importance of model specification when working with highly correlated aggregate economic variables.



> \*\*Important:\*\* These results describe statistical associations and should not be interpreted as causal effects.



\## Visualizations



The project includes visualizations of:



\- Real personal income versus personal consumption expenditure

\- Average personal consumption expenditure over time

\- Average real personal income over time

\- State-level differences in average personal consumption expenditure



The exported figures are available in \[`results/figures/`](results/figures/).



\## Results



Selected analysis outputs are also exported as CSV files for easier review and reuse:



\- \[`Descriptive statistics`](results/tables/descriptive\_statistics.csv)

\- \[`Correlation matrix`](results/tables/correlation\_matrix.csv)

\- \[`Model comparison`](results/tables/model\_comparison.csv)



\## Tools



\- Python

\- Pandas

\- NumPy

\- SciPy

\- Matplotlib

\- `linearmodels`

\- Google Colab

\- GitHub



\## Repository Structure



```text

household-consumption-income-dynamics/

├── README.md

├── notebook/

│   ├── PORTFOLIO\_00.ipynb

│   ├── PORTFOLIO\_01.ipynb

│   └── PORTFOLIO\_02.ipynb

├── documentation/

├── results/

│   ├── figures/

│   └── tables/

├── data/

│   └── PANEL\_DATA\_US.xlsx

└── requirements.txt



\## Reproducibility



The analysis was developed in Google Colab using Python.



The dataset is included in the repository under `data/`, while the required Python packages are listed in `requirements.txt`.



To reproduce the analysis:



1\. Clone the repository.

2\. Open the portfolio notebook in Google Colab or a compatible Jupyter environment.

3\. Install the required packages.

4\. Run the notebook from top to bottom.



The notebook loads the dataset from the repository and generates the analysis, visualizations, and selected exported results.



\## Limitations



The results should be interpreted with several limitations in mind:



\- The analysis identifies \*\*associations rather than causal effects\*\*.

\- The data are aggregated at the U.S. entity level rather than representing individual households.

\- Several aggregate economic variables are highly correlated, which can affect coefficient stability across specifications.

\- The estimated income-consumption relationship varies across model specifications and scaling approaches.

\- The analysis covers the \*\*2008–2024\*\* period and may not generalize to other time periods.

