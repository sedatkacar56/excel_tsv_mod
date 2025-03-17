# **excel_tsv_mod**

### **Overview**
`excel_tsv_mod` is an R package designed for efficient data analysis and visualization, particularly for handling **Excel** and **TSV (Tab-Separated Values)** datasets. It provides functions for **statistical analysis, data manipulation, and automated visualization** to streamline research workflows.

---

## **📌 Functions Included**
This package includes various functions for statistical computations and data visualization:

### **📝 Annotation & Visualization**
- **`annotationsplayableast`** – Adds statistical significance annotations (e.g., asterisks) to plots.
- **`boxplotwithasterisks`** – Generates boxplots with asterisks indicating statistical significance.
- **`differentasterisks`** – Customizes asterisks to denote varying significance levels.
- **`playwithasterisks`** – Provides interactive tools to modify statistical markers in plots.
- **`simpleboxplotwithstatistics`** – Creates boxplots with statistical summaries.

### **📊 Data Processing & Statistics**
- **`auto_graph_record`** – Automates the generation and saving of plots based on specified parameters.
- **`excel_columns`** – Converts between Excel column names and indices for easy manipulation.
- **`exceleautotukey`** – Performs **Tukey’s HSD test** for post-hoc analysis following ANOVA.
- **`normalized_gene_expression`** – Normalizes gene expression data for cross-sample comparisons.
- **`tukeyandboxplot`** – Integrates **Tukey's test results** into boxplots for deeper insights.

---

## **📥 Installation**
To use `excel_tsv_mod`, clone the repository and source the functions in your R session:

```r
# Clone the repository
git clone https://github.com/sedatkacar56/excel_tsv_mod.git

# Set working directory
setwd("path_to_cloned_repository")

# Source a specific function
source("path_to_function/function_name.R")

