# Androgen receptor transcriptomics + docking (GSE216372)

This repository contains an independent, reproducible re-analysis of a public skeletal-muscle transcriptomics dataset (NCBI GEO: GSE216372) and a molecular docking workflow using AutoDock Vina for androgen receptor ligand binding (with cross-receptor comparison to ERα and GR).

## What I did (high-level)
1. Retrieved differential expression results from GEO (GSE216372).
2. Filtered DE genes using adjusted p-value < 0.05 and |log2FC| ≥ 0.5.
3. Performed pathway enrichment (Enrichr; KEGG 2021 Human).
4. Generated summary figures (volcano plot, heatmap, enrichment bar plot).
5. Ran docking and summarized best-scoring affinities across receptors.

## Key outputs
- Manuscript PDF(s): full + anonymized versions
- Processed DE gene lists and enrichment inputs/outputs
- Figures used in the manuscript (PNG)
- Jupyter notebook(s) used to generate plots/tables

## Data sources
- GEO dataset: GSE216372 (public)
- Enrichment: Enrichr (KEGG 2021 Human)
- Docking: AutoDock Vina v1.2.7 (scores reported in kcal/mol)

## Notes
- Docking scores are *predicted* affinities (kcal/mol), not experimental binding free energies.
- All results are intended to be hypothesis-generating.
