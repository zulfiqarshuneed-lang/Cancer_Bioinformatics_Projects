# Cancer Bioinformatics: Transcriptomic Analysis & Molecular Docking

## Overview

This repository documents my learning journey in computational cancer biology, progressing from foundational transcriptomic analysis to the application of real-world bioinformatics workflows and structure-based drug discovery. The projects demonstrate how publicly available biological datasets and computational tools can be integrated to investigate cancer-associated molecular alterations and potential therapeutic targets.

---

# Repository Structure

## Project 1 — Introduction to Differential Gene Expression Analysis

**Objective**

Develop a foundational understanding of transcriptomic data analysis by simulating differential gene expression between normal and cancer-like conditions.

### Methods

- Simulated gene expression data using Python
- Calculated log fold change (logFC)
- Performed statistical significance testing
- Generated volcano plots and heatmaps
- Identified highly expressed candidate genes

## Example Outputs

### Volcano Plot

![Volcano Plot] [<img width="576" height="455" alt="image" src="https://github.com/user-attachments/assets/ee9ae2bf-d9ef-4ea1-a638-dcc6885d5932" />]

### Heatmap
![Heatmap] [<img width="542" height="435" alt="image" src="https://github.com/user-attachments/assets/9de2d94a-2d84-47f2-b4bf-55abad0ee248" />]

### Skills Learned

- Gene expression analysis
- Volcano plot interpretation
- Heatmap visualization
- Biological interpretation of transcriptomic data

---

## Project 2 — Differential Gene Expression Analysis Using Public GEO Data

**Research Question**

Which genes are differentially expressed between normal and cancer samples?

### Dataset

- **NCBI Gene Expression Omnibus (GEO)**
- **Dataset:** GSE15852

### Workflow

```
GEO Dataset
      │
      ▼
Download Expression Data (GEOparse)
      │
      ▼
Pre-processing
      │
      ▼
Differential Expression Analysis
      │
      ▼
Statistical Testing
      │
      ▼
Visualization
 ├── Volcano Plot
 ├── Heatmap
 └── Top Differentially Expressed Genes
      │
      ▼
Biological Interpretation
```
## Example Outputs

### Volcano Plot

![Volcano Plot] [<img width="545" height="470" alt="image" src="https://github.com/user-attachments/assets/e64c4f3b-8235-46b1-95e1-7e55e4b6b902" />]

### Heatmap

![Heatmap] [<img width="662" height="525" alt="image" src="https://github.com/user-attachments/assets/9d85b525-a87d-4629-a084-112ee6ba9282" />]

## Top Differentially Expressed Transcripts

| Rank | Transcript (Probe ID) | Log Fold Change (logFC) | p-value | −log10(p-value) |
|-----:|------------------------|-------------------------:|---------:|----------------:|
| 1 | 213614_x_at | 4711.96 | 2.23 × 10⁻¹² | 11.65 |
| 2 | 212869_x_at | 4057.39 | 1.60 × 10⁻⁹ | 8.79 |
| 3 | 206559_x_at | 4003.52 | 3.86 × 10⁻¹¹ | 10.41 |
| 4 | 212284_x_at | 3872.98 | 8.16 × 10⁻⁹ | 8.09 |
| 5 | 200062_s_at | 3777.09 | 8.49 × 10⁻¹³ | 12.07 |
| 6 | 200633_at | 3746.92 | 3.10 × 10⁻¹⁰ | 9.51 |
| 7 | 212391_x_at | 3550.81 | 3.63 × 10⁻⁸ | 7.44 |
| 8 | 204892_x_at | 3442.48 | 6.64 × 10⁻¹⁰ | 9.18 |
| 9 | 200717_x_at | 3423.50 | 2.68 × 10⁻¹⁰ | 9.57 |
| 10 | 213583_x_at | 3386.87 | 5.23 × 10⁻¹⁰ | 9.28 |

### Python Libraries

- GEOparse
- pandas
- NumPy
- SciPy
- matplotlib
- seaborn

### Key Results

- Downloaded and analysed a public breast cancer transcriptomic dataset.
- Identified differentially expressed transcript probes using statistical analysis.
- Generated volcano plots and heatmaps to visualize transcriptomic changes.
- Ranked candidate biomarkers based on expression differences and statistical significance.

---

## Project 3 — Computational Analysis of EGFR–Ligand Interactions

**Research Question**

Can computational molecular docking identify bioactive compounds that exhibit favourable binding affinity toward EGFR, a key therapeutic target in cancer?

### Methods

- Selected EGFR as the target protein.
- Performed molecular docking using CB-Dock2 (AutoDock Vina).
- Compared docking scores across predicted binding cavities.
- Interpreted protein–ligand interactions.

### Workflow

```
Differential Gene Expression Analysis
              │
              ▼
Identification of Cancer-Associated Target (EGFR)
              │
              ▼
Selection of Candidate Ligands
              │
              ▼
Molecular Docking (CB-Dock2 / AutoDock Vina)
              │
              ▼
Binding Affinity Comparison
              │
              ▼
Biological Interpretation
```
### Docking Scores

| Binding Site | Vina Score (kcal/mol) |
|--------------|----------------------:|
| Cavity 2 | **−7.3** |
| Cavity 1 | −7.1 |
| Cavity 3 | −6.7 |
| Cavity 4 | −6.3 |
| Cavity 5 | −6.3 |

### Key Findings

- Predicted favourable ligand binding to EGFR.
- Identified the strongest interaction at **Cavity 2** with a docking score of **−7.3 kcal/mol**.
- Demonstrated the use of molecular docking as a computational approach for early-stage drug discovery.

---

# Technologies & Tools

### Programming

- Python
- Google Colab

### Bioinformatics

- GEOparse
- pandas
- NumPy
- SciPy

### Visualization

- matplotlib
- seaborn

### Molecular Docking

- CB-Dock2
- AutoDock Vina
- Protein Data Bank (PDB)
- PubChem

---

# Learning Outcomes

Through these projects, I developed practical skills in:

- Differential gene expression analysis
- Transcriptomic data processing
- Statistical analysis of biological datasets
- Scientific data visualization
- Molecular docking
- Protein–ligand interaction analysis
- Computational cancer biology
- Reproducible bioinformatics workflows

---

# Future Improvements

- Perform differential expression analysis using Bioconductor (limma/edgeR).
- Conduct Gene Ontology (GO) and KEGG pathway enrichment analyses.
- Annotate transcript probes with gene symbols.
- Validate candidate biomarkers using external datasets.
- Perform molecular dynamics simulations to validate docking results.

---

## Author

**Shuneed Zulfiqar**

Biotechnology Graduate | Bioinformatics | Computational Biology | Cancer Genomics | Structure-Based Drug Discovery
