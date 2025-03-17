excel_tsv_mod
excel_tsv_mod is a collection of R functions aimed at simplifying data analysis and visualization tasks, especially when working with Excel and TSV data formats. The functions provided assist in generating various plots, performing statistical analyses, and automating repetitive tasks to enhance productivity.​

Functions Included
annotationsplayableast

Description: Facilitates the creation of annotation tables for plots, allowing for the addition of statistical significance indicators (e.g., asterisks) to visualizations.​
cran.r-project.org
auto_graph_record

Description: Automates the process of generating and saving plots based on specified parameters, streamlining the workflow of data visualization.​
boxplotwithasterisks

Description: Generates boxplots with asterisks indicating statistical significance between groups, providing a clear visual representation of differences.​
differentasterisks

Description: Allows customization of asterisks in plots to represent varying levels of statistical significance, enhancing the interpretability of results.​
excel_columns

Description: Provides utilities for handling Excel columns, such as converting between column names and indices, facilitating data manipulation tasks.​
exceleautotukey

Description: Performs Tukey's Honest Significant Difference test on Excel data, aiding in post-hoc analysis following ANOVA.​
normalized_gene_expression

Description: Processes gene expression data to normalize values, ensuring comparability across samples and conditions.​
playwithasterisks

Description: Offers interactive tools to add and customize asterisks in plots, allowing users to highlight significant findings effectively.​
simpleboxplotwithstatistics

Description: Creates simple boxplots accompanied by statistical summaries, providing quick insights into data distributions and differences.​
tukeyandboxplot

Description: Combines Tukey's test results with boxplots, offering a comprehensive view of data variability and group comparisons.
Installation
To utilize these functions, clone the repository and source the desired functions into your R environment:​

r
Copy code
# Clone the repository
git clone https://github.com/sedatkacar56/excel_tsv_mod.git

# Set working directory to the cloned repository
setwd("path_to_cloned_repository")

# Source a specific function
source("path_to_function/function_name.R")
Usage
After sourcing the functions, you can call them directly in your R scripts. For example:​

r
Copy code
# Assuming 'boxplotwithasterisks' has been sourced
boxplotwithasterisks(data, x_var, y_var, group_var)
Replace data, x_var, y_var, and group_var with your dataset and respective variables.​

Contributions
Contributions to enhance the functionality of this repository are welcome. Feel free to fork the repository, make improvements, and submit pull requests.​

License
This project is licensed under the MIT License. See the LICENSE file for details.​

Note: The descriptions provided above are based on typical functionalities inferred from the function
