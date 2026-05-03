🧬 Single-Cell RNA-seq Analysis of Melanoma

Cell Type Annotation & Cell–Cell Communication in Tumor Microenvironment

📌 Project Overview

This project presents a complete single-cell RNA sequencing (scRNA-seq) analysis pipeline of melanoma tumor samples with a focus on understanding the tumor immune microenvironment.

The workflow integrates:

Cell type identification and annotation
Differential gene expression analysis
Ligand–receptor-based cell–cell communication inference
Pathway-level signaling interpretation

The goal is to uncover how immune and tumor cells interact and how signaling pathways contribute to immune activation and immune suppression.

🧪 Biological Question

How do immune cells and tumor cells communicate in the melanoma microenvironment, and which signaling pathways dominate this interaction?

⚙️ Workflow Summary

The analysis follows a standard scRNA-seq pipeline:

1. Quality Control & Preprocessing
Filtering low-quality cells and genes
Normalization and log transformation
Feature selection

3. Dimensionality Reduction & Clustering
PCA for feature reduction
UMAP visualization
Leiden clustering for cell population identification

5. Cell Type Annotation
Marker gene-based scoring
Cluster-level annotation refinement
Identification of major immune cell populations

7. Differential Gene Expression (DEG)
Cluster-wise differential expression
Identification of marker genes per cell type
Statistical filtering (FDR-controlled)

9. Cell–Cell Communication Analysis
Ligand–receptor inference using LIANA framework
Integration of multiple methods (CellPhoneDB, Connectome, NATMI, etc.)
Interaction scoring and filtering

11. Pathway-Level Analysis
Mapping ligand–receptor interactions to signaling pathways
Identification of immune-related pathways
Ranking of communication strength across pathways

📊 Dataset Summary

Total cells: ~4,600
Cell types identified: 6 major immune populations
Clusters detected: ~18 Leiden clusters
Identified cell types:
CD4⁺ T cells
CD8⁺ T cells
NK cells
Naive B cells
CD14⁺ Monocytes
Dendritic cells

🔬 Key Findings

🧬 1. Immune activation signals

Strong Chemokine signaling
Active Interferon (IFN) signaling

These indicate immune cell recruitment and activation in the tumor microenvironment.

❗ 2. Immune suppression signals

PD-1 checkpoint pathway
TGF-β signaling

These pathways suggest tumor-driven immune suppression and T-cell exhaustion.

🔗 3. Cell–cell communication landscape

T cells act as central communication hubs
Monocytes and dendritic cells are major signal senders
NK cells strongly interact with CD8 T cells

⚡ 4. Key ligand–receptor interactions

HLA-B → CD3D
HLA-B → CD8A

Indicating strong antigen presentation and immune recognition signals.

📈 Pathway-Level Insights

Top enriched communication pathways:

Chemokine signaling
Interferon signaling
PD-1 immune checkpoint
TNF signaling
TGF-β signaling

🧠 Biological Interpretation

The melanoma tumor microenvironment shows a dual immune state:

Active immune response (IFN and chemokine signaling)
Simultaneous immune suppression (PD-1 and TGF-β pathways)

This suggests that while immune cells are recruited and active, tumor-mediated checkpoint signaling likely inhibits effective anti-tumor immunity.

📊 Key Outputs

This repository includes:

📁 Clustering results (Leiden)
📁 Cell type annotations
📁 Differential expression tables
📁 Ligand–receptor interaction results (LIANA)
📁 Pathway-level summaries

📊 High-resolution figures:

UMAP plots
Interaction networks
Heatmaps
Bubble plots

🧰 Tools & Packages

Python (3.x)
Scanpy
LIANA
Pandas / NumPy
Matplotlib / Seaborn


📌 Applications

This pipeline can be used for:

Tumor microenvironment studies
Immuno-oncology research
Biomarker discovery
Drug target identification
Cell communication studies in cancer

💡 Future Improvements

Integration with spatial transcriptomics
Multi-sample comparative analysis
Survival correlation (clinical data)
Machine learning-based cell state classification

👤 Author

Kavoos Momeni

Bioinformatics & Genomics Analysis

Focused on:

Single-cell RNA-seq
Tumor microenvironment analysis
Computational biology pipelines

📬 Contact : kavoosmomeni@gmail.com

⭐ Acknowledgements

This project uses open-source tools including Scanpy and LIANA for single-cell and communication analysis.
