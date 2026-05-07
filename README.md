# EditScreen

**Universal base editing and CRISPR screen analysis tool**

Analyze, visualize, and compare CRISPR/base editing screens without switching between 5+ tools. Single unified interface for filtering, statistics, 3D protein mapping, and multi-screen comparison.

## Features

- **Base editing screen analysis** — Mutation categorization, statistical filtering (Z-score, FDR, fold change)
- **Genome-wide CRISPR screens** — Gene-level hit identification and volcano plots
- **3D protein visualization** — Map hits directly onto PDB structures
- **Multi-screen comparison** — Compare hits across experiments with overlay and correlation plots
- **Flexible visualization** — Scatter, volcano, heatmap, lollipop, distribution views
- **Batch processing** — Analyze multiple screens; export results for cloning
- **Pathway analysis integration** — One-click GO/KEGG enrichment (Enrichr, g:Profiler, STRING)

## Quick Start

### Online (no installation)
1. Go to: https://parijat-sarkar.github.io/EditScreen/
2. Upload your Excel file
3. Map columns
4. Adjust cutoffs and download results

### Data Format

**Required columns:**
- `Guide ID` — Unique identifier for each guide
- `Gene Name` — Target gene (or protein for base editing screens)

**Optional columns:**
- `Guide Sequence`
- `Residue Number` or `Predicted Mutations` (for base editing)
- `Fold Change` — log2 scale preferred
- `P-value` or `FDR` — raw (0–1) or –log10 transformed
- `Z-score` or `score`
- `High in Treatment` — Boolean (TRUE/FALSE)

**File format:** .xlsx, .xls, or .csv


## Usage Examples

### Base Editing Screen
1. Upload screen Excel file
2. Map: Guide ID, Gene Name, Mutation Category columns
3. Add statistics (Z-score, Fold Change, FDR)
4. Select protein from library or upload custom sequence
5. Filter by mutation type and significance
6. View 3D structure hits
7. Download oligos for cloning

### Genome-Wide CRISPR Screen
1. Upload gene-level results
2. Map: Gene Name, Fold Change, P-value columns
3. Choose volcano plot or table view
4. Filter by fold change and significance
5. Export gene list for pathway analysis

### Multi-Screen Comparison
1. Upload two screen files
2. Map columns for both
3. View common vs. unique hits
4. Download comparison report

## 3D Structure Visualization

Map screen hits directly onto PDB structures:
- Load structure from RCSB or upload .pdb file
- Color by: mutation category, cutoff status, or metric value
- Adjust chain and residue numbering offset
- Download colored PDB or PNG snapshot

## Citation

If you use EditScreen in your research, please cite:
Sarkar, P. (2026). EditScreen: Universal base editing and CRISPR screen analysis tool. GitHub: https://github.com/parijat-sarkar/EditScreen

## FAQ

**Q: Is my data private?**
A: EditScreen runs entirely in your browser. No data is uploaded to any server.

**Q: Can I use this for large screens (100K+ guides)?**
A: Yes, but performance depends on your computer. Start with filtering to reduce data size.

**Q: What statistics does it support?**
A: Z-score, fold change, P-value, FDR, and custom metrics.

**Q: Can I batch analyze multiple files?**
A: Yes, use Multi-Screen Comparison mode.

**Q: How do I report bugs or request features?**
A: [Open an issue](https://github.com/parijat-sarkar/EditScreen/issues)

## Contributing

Found a bug? Have an idea? Want to contribute?

[See CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

MIT License — see [LICENSE](LICENSE) file

## Contact

Questions or suggestions? Open an [issue](https://github.com/parijat-sarkar/EditScreen/issues) or reach out.

---

**Made with ❤️ for genome editing researchers**
