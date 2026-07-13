# Food Security, Health and Development in Asia

Interactive data analysis of food security, public health, nutrition and socioeconomic development across Asian countries.

[![Live Report](https://img.shields.io/badge/Live%20Report-View%20Interactive%20Analysis-2563eb?style=for-the-badge)](https://beepboopvictor.github.io/asia-food-security-analysis/)

![Project overview](assets/cover.png)

## Project overview

This project explores how food security, nutrition, public health and socioeconomic indicators are related across Asian countries.

The objective is not only to visualize the available data, but also to identify meaningful patterns, compare countries and periods, study relationships between variables and communicate the limitations of the analysis clearly.

The final result is an interactive HTML report developed in R and published through GitHub Pages.

## Live demo

The complete interactive analysis is available here:

**[Open the interactive report](https://beepboopvictor.github.io/asia-food-security-analysis/)**

The report includes interactive charts, geographic visualizations, correlation analysis and dimensionality reduction.

## Research questions

The analysis focuses on the following questions:

* How have food security and health indicators evolved across Asian countries?
* Which countries present the most significant differences?
* What relationships exist between nutrition, mortality, economic development and population indicators?
* How does the level of aggregation affect the interpretation of correlations?
* Can dimensionality reduction reveal common structures among the indicators?

## Main findings

The analysis highlights several relevant patterns:

* Health, nutrition and development indicators are strongly interconnected, although the strength of these relationships depends on the aggregation level.
* Country-level averages may hide temporal variation and internal differences.
* Correlation values must be interpreted carefully, as they do not imply causal relationships.
* Variable transformations can substantially change the apparent relationship between indicators.
* The first three principal components explain approximately **87.9% of the total variance**, allowing most of the dataset's structure to be represented in a lower-dimensional space.
* Geographic and socioeconomic context remains essential when comparing countries.

## Interactive visualizations

The report combines static statistical graphics with interactive visualizations created using Plotly, Highcharter and Leaflet.

### Geographic analysis

![Interactive geographic analysis](assets/map.png)

The geographic visualizations make it possible to compare indicators between countries and identify spatial patterns that would be difficult to detect in traditional tables.

### Principal Component Analysis

![Principal Component Analysis](assets/pca.png)

Principal Component Analysis was used to summarize the information contained in multiple correlated variables and explore similarities between countries.

## Methodology

The project follows a reproducible data analysis workflow:

1. Data loading and inspection.
2. Data cleaning and preparation.
3. Exploratory data analysis.
4. Temporal and geographic comparison.
5. Correlation analysis.
6. Variable transformation.
7. Principal Component Analysis.
8. Interactive data visualization.
9. Critical interpretation of results and limitations.
10. Publication as a self-contained HTML report.

Special attention was given to distinguishing between:

* aggregated country-level indicators;
* country-year observations;
* transformed and non-transformed variables;
* statistical association and causal interpretation.

## Technologies

* **R**
* **R Markdown**
* **Shiny**
* **ggplot2**
* **Plotly**
* **Highcharter**
* **Leaflet**
* **dplyr**
* **tidyr**
* **FactoMineR / PCA**
* **HTML**
* **GitHub Pages**

## Repository structure

```text
.
├── index.html
├── P1.Rmd
├── shiny.Rmd
├── README.md
└── assets
    ├── cover.png
    ├── map.png
    └── pca.png
```

### Main files

* `index.html`: final interactive report published with GitHub Pages.
* `P1.Rmd`: reproducible analysis and report generation.
* `shiny.Rmd`: interactive dashboard implementation.
* `assets/`: screenshots and visual resources used in the README.

## Reproducibility

The analysis was developed using R Markdown to combine code, results, visualizations and interpretation in a reproducible document.

To reproduce the project locally:

1. Clone the repository.
2. Open `P1.Rmd` in RStudio.
3. Install the required R packages.
4. Verify that the datasets are available in the expected paths.
5. Knit the document to HTML.

Some elements of the Shiny dashboard may require running an R session with the necessary packages and datasets installed.

## Limitations

This project is primarily exploratory.

The results should therefore be interpreted with the following limitations in mind:

* Correlation does not imply causation.
* Data availability may differ between countries and years.
* Aggregated national indicators can conceal regional or social inequalities.
* The sum of national rates does not represent a continental mortality total or a valid continental rate.
* Differences in data collection methods may affect comparisons.
* Missing values and transformations may influence the resulting relationships.
* Principal components summarize variance but do not necessarily represent directly observable real-world factors.

## Future improvements

Possible extensions include:

* updating the datasets with more recent observations;
* adding confidence intervals and statistical significance tests;
* incorporating regional and subnational data;
* developing predictive models;
* deploying the complete Shiny application;
* improving accessibility and mobile interaction;
* adding automated data pipelines;
* comparing Asian countries with other world regions.

## Author

**Víctor Gil Bernal**

Graduate in Data Science and Engineering from the University of Las Palmas de Gran Canaria.

Interested in data engineering, data science, applied artificial intelligence, automation and the development of reproducible analytical products.

## Contact

* LinkedIn: `www.linkedin.com/in/victor-gil-bernal`
* GitHub: `https://github.com/BeepBoopVictor`

## License

This repository is intended for educational, academic and portfolio purposes.

The source datasets may be subject to their own licenses and usage conditions.
