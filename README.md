🧬 Single-Cell RNA-seq Analysis of Melanoma
Cell–Cell Communication & Immune Signaling
📌 Project Overview

This project performs a full single-cell RNA-seq analysis pipeline on melanoma data, with a focus on:

Cell type identification
Differential gene expression
Cell–cell communication (CCI)
Pathway-level signaling analysis
⚙️ Methods

The analysis includes:

Quality control & normalization
Leiden clustering
Cell type annotation
Differential expression analysis (DEG)
Cell–cell communication using LIANA
Pathway-level interpretation
📊 Key Results
Identified 6 major immune cell types
Detected 3,800+ significant DEGs
Inferred 25,000+ ligand–receptor interactions
Highlighted key pathways:
Chemokine signaling
IFN signaling
PD-1 checkpoint
TGF-β signaling
🔬 Biological Insight

Tumor-associated immune cells show:

Active immune signaling (chemokines, interferon)
Concurrent immune suppression (PD-1, TGF-β)

➡️ Suggesting an immune-active but suppressed tumor microenvironment

🖼️ Key Figures
UMAP Clustering

Interaction Network

Pathway Heatmap

📁 Outputs
results/*_DEG_results.csv
results/*_liana_results.csv
results/*_pathway_ranking.csv
🧪 Tools & Libraries
Python
Scanpy
LIANA
Pandas / NumPy
Matplotlib
