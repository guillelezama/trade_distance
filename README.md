# Latin American Trade Analysis Notebook

## Overview
This repository contains a Jupyter notebook designed for analyzing trade relationships between six Latin American countries and other countries worldwide. The analysis focuses on the exports and imports of goods at the ISIC Rev. 4 level using data from UN Comtrade for the year 1995.

## Data Sources
- **UN Comtrade Data (1995):** The primary dataset used for this analysis, comprising detailed trade data for various countries.
- **HS to ISIC Conversion Key:** A conversion key from HS (Harmonized System) classification to ISIC (International Standard Industrial Classification) classification, obtained from the OECD website. This key is essential for aligning the trade data with the ISIC Rev. 4 classification. The conversion key can be downloaded [here](https://www.oecd.org/sti/ind/ConversionKeyBTDIxE4PUB.xlsx).

## Repository Structure
- `trade_data/`: This folder contains all the trade data downloaded from UN Comtrade.
- `Latin_American_Trade_Analysis.ipynb`: The Jupyter notebook where all the analysis is performed.

## Notebook Workflow
1. **Data Import:** The notebook imports data into four distinct datasets:
   - Latin American countries' imports
   - Latin American countries' exports
   - Rest of the world's imports
   - Rest of the world's exports
2. **Conversion to ISIC Classification:** The trade data, initially in HS classification, is converted to the ISIC Rev. 4 classification, aligning it with international industrial standards.
3. **Sector-wise Trade Share Computation:** For each country, the notebook calculates the share of exports and imports in each sector, providing insights into the trade patterns.
4. **Similarity Analysis:** Using methods like cosine similarity, Euclidean distances, and Pearson correlations, the notebook generates a list of the top 5 countries that show the most similarity with each Latin American country in terms of imports and exports.

## Usage
To use this notebook:
1. Ensure you have Jupyter Notebook or JupyterLab installed.
2. Clone this repository.
3. Navigate to the repository directory and launch Jupyter Notebook or JupyterLab.
4. Open `Similarities_Exports_Imports.ipynb` and run the cells to perform the analysis.

## Requirements
- Python 3.x
- Jupyter Notebook or JupyterLab
- Relevant Python libraries as listed in the notebook (e.g., pandas, scikit-learn, scipy)
