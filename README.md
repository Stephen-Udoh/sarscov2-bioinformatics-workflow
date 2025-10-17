# sarscov2-bioinformatics-workflow
Workflow for SARS-CoV-2 sequence analysis from BAM to FASTA, clade and lineage identification using Nextclade

Most steps were performed on the **Linux command line**, with Python used for result visualization and summary statistics.

---

## ⚙️ Workflow Summary

1. **Quality Control**  
   - `fastqc` and `trimmomatic` for read quality trimming  
   - `bwa` for reference alignment  

2. **Mapping and Consensus Generation**  
   - `samtools` for BAM indexing and flagstat  
   - `ivar` for variant calling and consensus FASTA generation  

3. **Clade and Lineage Assignment**  
   - `nextclade` (with `nextclade_pango` dataset) for SARS-CoV-2 lineage and clade analysis  

4. **Data Visualization**  
   - Python and Jupyter Notebook for summary plots and QC visualization  

---

## 🧰 Tools Used

| Tool | Version | Purpose |
|------|----------|----------|
| fastqc | latest | Quality control |
| trimmomatic | v0.39 | Read trimming |
| bwa | v0.7.17 | Sequence alignment |
| samtools | v1.19.2 | BAM/FASTA operations |
| ivar | v1.4.2 | Consensus and variant calling |
| nextclade | v3.2.4 | Clade and lineage assignment |

---

## 🐍 Python Dependencies

Listed in `requirements.txt`:
