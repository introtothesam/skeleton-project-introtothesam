# Gapminder: Data Wrangling, Visualization, and Hypothesis Testing

## **Project Overview**

This project focuses on **data wrangling, visualization, and statistical analysis** using the **Gapminder** dataset. The goal is to transform raw data into structured formats, generate meaningful visualizations, and conduct hypothesis testing to explore global economic trends over time. The project follows best practices for **reproducibility and modular workflow**, ensuring that each step is clearly documented and reusable.

## **Dataset**

The project utilizes the **Gapminder** dataset, which provides country-level data on **life expectancy, GDP per capita, and population** across multiple years. The dataset has been cleaned, transformed, and visualized using **dplyr, tidyr, stringr, and ggplot2**.

## **Research Questions**

1.  **How have life expectancy and GDP per capita changed over time across different regions?**
2.  **What is the relationship between GDP per capita and life expectancy?**
3.  **Does population size influence economic growth trends?**

## **Cloning the Repository**

To clone this repository and navigate into the project directory, run:

``` bash
git clone https://github.com/introtothesam/skeleton-project-introtothesam.git
cd skeleton-project
```

## **Repository Structure**

To generate the repository structure, run the following command in the terminal:

``` bash
tree 
```

This will output the directory tree structure:

```         
.
├── README.md                 # Project description          
├── data/                     # Directory for datasets
│   ├── processed/            
│   │   └── gm-wrangled-goal.csv  # Post-wrangling Gapminder dataset 
│   └── raw/                
│       └── gapminder.csv     # Raw Gapminder dataset
├── references/               # Bibliography and external sources
├── reports/                  # Generated reports from analyses
├── scripts/                  
│   ├── plotting-function-map.R  # Interactive plotting functions (scatter, bar, map)
│   └── recreate-level-2.qmd  # Data wrangling and visualization
└── skeleton-project.Rproj     # R project configuration file
```

## **Installation Requirements**

Before running the scripts, ensure the following R packages are installed:

``` r
install.packages(c("tidyverse", "ggplot2", "ggiraph", "patchwork", "sf", "scales", "broom", "dplyr", "tidyr", "stringr", "forcats"))
```

## Running the Workflow

1.  Open `skeleton-project.Rproj` in **RStudio**.

2.  Run the scripts in the following order:

    -   **`plotting-function-map.R`**: Defines custom plotting functions used for visualization.
    -   **`recreate-level-2.qmd`**: Performs Level 2 data wrangling, visualization, and analysis.

## **Analysis Methods**

The project applies various data analysis techniques, including:

### **Data Wrangling**

-   **Cleaning and restructuring**: Using `dplyr`, `tidyr`, and `stringr` to filter, rename, and reformat columns.
-   **Feature engineering**: Creating economic score variables, population ranks, and relative life expectancy measures.

### **Exploratory Data Analysis**

-   **Visualizing trends and distributions** using `ggplot2`.
-   **Creating interactive maps** with `ggiraph` and `ggplot2`.

### **Statistical Testing**

-   **T-tests** for comparing life expectancy across continents.
-   **ANOVA** for multi-group comparisons.
-   **Correlation analysis** between GDP per capita and life expectancy.
-   **Linear regression modeling** to assess economic indicators' impact on life expectancy.

## **Expected Outputs**

-   **Data Cleaning:** Transformed dataset saved as `gm.wrangled.csv`
-   **Visualizations:** Interactive plots stored in `reports/`
-   **Final Report:** Rendered in `reports/draft.html`

## **References**

-   **Gapminder Dataset:** <https://www.gapminder.org/data/>

## Author

-   **Chenyi Dai**
