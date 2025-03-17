SedatFunctions: A Collection of R Functions for Single-Cell Analysis

Overview

SedatFunctions is an R package designed to streamline single-cell RNA sequencing (scRNA-seq) analysis, providing essential functions for data processing, integration, visualization, and downstream analysis. The package is built around the Seurat framework and supports workflows for cell-type identification, trajectory inference, marker detection, and metadata handling.

Installation

To install SedatFunctions, clone the repository and load it in R:

# Install required dependencies
install.packages("devtools")

# Clone and install the package
library(devtools)
devtools::install_github("sedatkacar56/SedatFunctions")

# Load the package
library(SedatFunctions)

Functions & Usage

Below is a summary of the key functions available in SedatFunctions:

Data Processing

process_seurat_txtgz(): Save or load Seurat objects as .txt.gz files.

RNA_seurat(): Process and normalize an individual RNA dataset.

process_and_integrate(): Integrate multiple Seurat objects (up to 4 samples).

compute_group_averages(): Compute average gene expression per group.

scale_to_range(): Scale data between -2 and +2.

Metadata & Label Transfer

Transfer_Labels(): Transfer annotations from a reference dataset to a query Seurat object.

transfer_metadata(): Transfer selected metadata from one object to another.

swap_levels(): Swap factor levels in a Seurat metadata column.

modify_seurat_color(): Customize colors for cell types in a Seurat object.

Marker Detection & DEG Analysis

get_top_markers(): Identify top markers for each cluster.

run_deg_analysis(): Perform differential gene expression (DEG) analysis.

find_and_save_markers(): Find and export DEGs between experimental conditions.

Cell Type Annotation & Visualization

generate_celltype_more(): Summarize cell-type distribution across conditions.

generate_heatmap(): Generate heatmaps for gene expression.

plot_clusters(): Visualize clusters with DimPlot().

highlight_cells(): Highlight specific cell groups in a UMAP plot.

panel_of_images(): Create multi-panel image visualizations.

Trajectory & Dimensionality Reduction

run_monocle3_trajectory(): Perform trajectory analysis using Monocle3.

RunHarmonyIntegration(): Apply Harmony batch correction to Seurat objects.

Utilities

GOids(): Retrieve Gene Ontology (GO) terms for specified genes.

get_gene_info(): Fetch gene information from Ensembl.

write_functions_to_file(): Save a list of functions to an external R file.

save_cross_table(): Save a contingency table of metadata variables.

Example Usage

# Load the package
library(SedatFunctions)

# Create a Seurat object from a dataset
seurat_obj <- RNA_seurat(my_data)

# Find top markers
top_markers <- get_top_markers(seurat_obj)

# Generate a heatmap
heatmap_plot <- generate_heatmap(seurat_obj, genes = c("GAPDH", "ACTB"))

# Perform differential expression analysis
deg_results <- run_deg_analysis(seurat_obj, ident_pairs = list(c("Control", "Treated")))

Contribution

Feel free to contribute by submitting issues, feature requests, or pull requests on GitHub.

License

This package is distributed under the MIT License.

Author

Developed by Sedat Kacar

🚀 For more details, check out the function documentation using: ?function_name
