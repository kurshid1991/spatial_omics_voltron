## Spatial Omics Data Analysis with VoltRon
This repository contains R scripts demonstrating the use of VoltRon for spatial omics data analysis. The primary focus is on loading data, exploring metadata, visualizing molecules and cell clusters, and generating multilayer visualizations.

### Features
- Import and manage spatial omics data
- Visualize spatial distributions of molecules and cells
- Combine image channels for clear representation
- Perform interactive visualization of spatial data
- Create multilayer visualizations combining multiple assays and annotations

### Prerequisites
- R (version >= 4.0.0)
- VoltRon package installed
- Other recommended packages: ggplot2, dplyr, magrittr

**IMPORTANT NOTE: Please install the following dependencies first *before* installing VoltRon.**

- rhdf5: BiocManager::install(“rhdf5”)
- RBioFormats: BiocManager::install(“RBioFormats”) 
- Note: RBioFormats might be hard to install due to java dependency. Check https://github.com/BIMSBbioinfo/VoltRon/tree/dev?tab=readme-ov-file#dependencies for more information.
- Seurat: install.packages("Seurat")
- spacexr: devtools::install_github("dmcable/spacexr")
- ComplexHeatmap: BiocManager::install("ComplexHeatmap")
- HDF5Array: BiocManager::install("HDF5Array")
- HDF5DataFrame: devtools::install_github("BIMSBbioinfo/HDF5DataFrame")
- ImageArray: devtools::install_github("BIMSBbioinfo/ImageArray")
- BPCells: devtools::install_github("bnprks/BPCells/r@v0.3.0")

**Note: You may need to install BPCells *before* installing VoltRon**

- vitessceR: devtools::install_github("vitessce/vitessceR")
- basilisk: BiocManager::install("basilisk")
- ggnewscale: install.packages("ggnewscale")
- presto: devtools::install_github('immunogenomics/presto')

## Data
The repository includes the following datasets for demonstration purposes:

- merged_object
- melc_data
- xenium_data

## Code Overview
- Data Import and Exploration: Load sample data and inspect metadata.
- Image Handling: View and manipulate images, including channel combination for enhanced visualization.
- Visualization: Visualize cell clusters, molecules, and segment annotations using vrSpatialPlot.
- Multilayer Visualization: Overlay multiple data layers for a comprehensive view.

