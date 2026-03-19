# Climate Change Vulnerability Assessment (CCVA) - YPINB Notebook

## Overview

This Jupyter notebook (`ccva_ypinb.ipynb`) performs a comprehensive Climate Change Vulnerability Assessment (CCVA) for small-scale fisheries (SSFs) in Northern Madagascar. The analysis addresses key research questions related to vulnerability assessment, the role of sensitivity and adaptive capacity in explaining climate impacts, and prioritization of adaptation strategies.

## Research Questions

1. **Vulnerability Assessment**: How can climate change vulnerability be assessed among SSFs in Northern Madagascar? (Sections 1-4)
2. **Domain Analysis**: To what extent do Sensitivity and Adaptive Capacity domains explain variation in climate-related impacts at the household level, and how do these relationships differ between well-established LMMA (Locally Managed Marine Area) sites and LMMA sites with implementation in progress? (Section 5)
3. **Adaptation Strategies**: What strategies and actions should be prioritized to achieve optimal adaptation to climate change? (Recommendations)

## Methodology

The notebook employs:
- **Analytic Hierarchy Process (AHP)** for weighting indicators, domains, and dimensions
- **Household-level data analysis** for vulnerability indices
- **Statistical modeling** (e.g., logistic regression) to examine relationships
- **Data visualization** using matplotlib and plotly for charts and maps
- **Aggregation techniques** for combining raw and weighted vulnerability scores

## Data Structure

- **Input Data**: Located in `data/` folder, including CSV files for AHP scores, household data, and metadata
- **Outputs**: Generated in `output/` folder, including vulnerability indices, classification tables, and graphs

## Dependencies

Install required packages using:

```bash
pip install -r requirements.txt
```

Key libraries include:
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- scikit-learn
- jupyter

## Setup and Execution

1. **Environment Setup**:
   - Create a virtual environment: `python -m venv .venv`
   - Activate: `.venv\Scripts\Activate.ps1` (Windows)
   - Install dependencies: `pip install -r requirements.txt`

2. **Run the Notebook**:
   - Launch Jupyter: `jupyter notebook`
   - Open `notebook/ccva_ypinb.ipynb`
   - Execute cells sequentially

## Project Structure

```
ccva/
├── notebook/
│   └── ccva_ypinb.ipynb          # Main analysis notebook
├── data/                         # Input data files
│   ├── ahp_*.csv                 # AHP weighting data
│   ├── mdg_*.csv                 # Household vulnerability data
│   └── dimension_domain_indicator_metadata.csv
├── output/                       # Generated outputs
│   ├── graph/                    # Visualization outputs
│   └── table/                    # Classification and summary tables
├── scripts/                      # Additional scripts
├── requirements.txt              # Python dependencies
└── README.md                     # This file
```

## Key Variables and Outputs

- **Vulnerability Indices**: Computed at household, domain, and indicator levels
- **AHP Weights**: Expert and default weighting schemes
- **Statistical Models**: Logistic regression results for impact analysis
- **Visualizations**: Radar charts, bar plots, quadrant analyses

## Notes

- The notebook has been executed successfully with outputs including plots and statistical summaries.
- Some cells may require specific data paths; ensure the working directory is set to the project root.
- For detailed methodology, refer to the inline comments and markdown cells within the notebook.

## Contact

For questions or contributions, please refer to the project repository or contact the maintainer.