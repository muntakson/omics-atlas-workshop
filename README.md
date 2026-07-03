# 🧬 Omics Atlas — Hands-on Workshop

Interactive Google Colab notebooks that accompany **[Omics Atlas](https://omics.iotok.org)**, a molecular-genetics course. Practise the analyses from each chapter in Python, on **real** data — no install, runs in your browser.

## The dataset

The **airway** RNA-seq dataset (Himes *et al.*, 2014, *PLoS ONE*): four human airway smooth-muscle cell lines, each with a dexamethasone-treated and an untreated control sample (8 samples, ~38k genes). It is the canonical teaching dataset for differential expression.

## Notebooks

| # | Notebook | Chapter | Open |
|---|----------|---------|------|
| 1 | Exploring RNA-seq count data | Ch.1 — RNA-seq basics | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/muntakson/omics-atlas-workshop/blob/main/notebooks/01_rnaseq_explore.ipynb) |
| 2 | Differential expression with PyDESeq2 | Ch.2 — Practical guide | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/muntakson/omics-atlas-workshop/blob/main/notebooks/02_differential_expression.ipynb) |
| 3 | Pathway enrichment analysis | Ch.3 — Enrichment protocol | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/muntakson/omics-atlas-workshop/blob/main/notebooks/03_pathway_enrichment.ipynb) |
| 4 | Interpreting & visualizing enrichment | Ch.4 — Interpreting omics | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/muntakson/omics-atlas-workshop/blob/main/notebooks/04_interpreting_enrichment.ipynb) |
| 5 | Single-cell RNA-seq with Scanpy | Ch.5 — scRNA-seq best practices | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/muntakson/omics-atlas-workshop/blob/main/notebooks/05_single_cell.ipynb) |

Work through them in order — each builds on the last (counts → DEGs → pathways → enrichment map).

## Tools

`pandas` · `scikit-learn` · `PyDESeq2` · `gseapy` (Enrichr / GSEA) · `mygene` · `matplotlib` / `seaborn` · `networkx`

## Data files

- `data/airway_scaledcounts.csv` — gene × sample count matrix
- `data/airway_metadata.csv` — sample sheet (control / treated)
- `data/airway_deseq2_results.csv` — precomputed DESeq2 results (so notebooks 3–4 run standalone)

Data © the original authors; reproduced for education.
