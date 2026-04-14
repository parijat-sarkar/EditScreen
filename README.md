# EditScreen
Universal base editing and CRISPR screen analysis tool.

EditScreen is a browser-based interactive tool for analyzing base editing and CRISPR screening data. It supports both residue-level base editing datasets and genome-wide CRISPR or insertional mutagenesis screens, enabling flexible exploration of functional genomics results without requiring coding.

The app allows users to upload Excel or CSV files, map columns to relevant fields (such as guide IDs, mutations, or gene names), and configure statistical metrics including Z-score, fold change, p-value, and FDR. It provides multiple visualization modes such as scatter plots, lollipop plots, heatmaps, volcano plots, and tables, along with dynamic filtering and multi-screen comparison.

EditScreen also includes protein-level analysis, allowing mapping of mutations onto sequences, defining domains, and integrating structural context through 3D visualization using PDB files or AlphaFold Predictions.

All analysis runs locally in the browser with no backend required. Results can be exported as filtered datasets, SVG figures, or cloning-ready oligo sequences.

Author:
Parijat Sarkar,
Stanford University
