# RNA-seq Differential Expression Analysis of Multiple Sclerosis White Matter Brain Lesions

Analysis of the GEO dataset GSE138614 comparing gene expression between multiple sclerosis
white matter lesion samples and control white matter samples using DESeq2.

**Course:** ST2GEA - Genomics, Epigenetics and Applications  
**Author:** Kiroshan SIVAKUMAR - Student ID: 20221526  
**Professor:** MATHEW Mano Joseph  

---

## Repository Structure
```
.
├── MS_RNAseq_Analysis.Rmd    # Main analysis document (RMD)
├── MS_RNAseq_Analysis.html   # Rendered HTML report (HTML)
│
├── data/
│   ├── GSE138614_raw_counts_GRCh38.p13_NCBI.tsv    # raw count matrix (TSV)
│   └── Human.GRCh38.p13.annot.tsv                  # gene annotation (TSV)
│
└── results/
    ├── figures/    # All generated plots (PNG)
    └── tables/     # All generated tables (CSV)
```
---

## How to Run

1. Clone the repository

```bash
git clone https://github.com/Genomics-Epigentics-EFREI-Promo2027/SIVAKUMAR-KIROSHAN-GSE138614.git
cd SIVAKUMAR-KIROSHAN-GSE138614
```

2. Download the data from GEO

The raw count matrix and annotation file must be downloaded from
[GSE138614](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE138614)
and placed in the `data/` folder.

3. Render the R Markdown document

Open `MS_RNAseq_Analysis.Rmd` in RStudio and click **Knit**, or run in R:

```r
rmarkdown::render("MS_RNAseq_Analysis.Rmd")
```

All required packages are installed automatically at the start of the document.

---

## Reference

Elkjær ML et al. (2019). Molecular signature of different lesion types in the brain
white matter of patients with progressive multiple sclerosis.
*Acta Neuropathologica Communications*, 7(1):107.
doi: [10.1186/s40478-019-0855-7](https://doi.org/10.1186/s40478-019-0855-7)
