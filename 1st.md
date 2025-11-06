# 🧬 Genetic Information in Prokaryotic and Eukaryotic Cells & High-Throughput Technologies

---

## 1. Organization of Genetic Material

**Genome:** Complete set of genetic material (DNA/RNA), including genes, non-coding, repetitive, and intergenic regions.

### Historical Milestones
- 1920s – “Genome” term coined (genes + chromosomes).
- 1953 – DNA double-helix model proposed by Watson & Crick.
- 1977 – Sanger sequencing introduced.
- 2003 – Human Genome Project completed.
- 2022 – Telomere-to-Telomere (T2T) assembly achieved (nearly gapless human genome).

**Significance:** Understanding genome organization reveals evolution, gene regulation, and disease mechanisms.

---

## 2. Genome Size and the C-Value Paradox

**C-Value:** Amount of DNA in a haploid genome.

**C-Value Paradox:** Genome size does not correlate with organismal complexity.
- Example: Some plants have more DNA than humans but similar gene counts.

### Examples

| Organism | Genome Size | Gene Count |
|-----------|--------------|------------|
| E. coli | ~4.6 Mb | ~4,300 |
| Yeast | ~12 Mb | ~6,000 |
| Human | ~3.2 Gb | ~25,000–30,000 |
| Lily | ~120 Gb | Similar to human |

**Explanation:** Due to repetitive DNA, transposons, and non-coding regions.

---

## 3. Chromosomal and Extra-Nuclear DNA

### Eukaryotes
- **Nuclear DNA:** Linear chromosomes.
- **Mitochondrial/Chloroplast DNA:** Circular, prokaryotic-like.
- **Endosymbiotic theory:** Organelles originated from ancient bacteria.

### Prokaryotes
- **Single circular chromosome** in nucleoid.
- **Plasmids:** Small, self-replicating DNA with accessory genes (e.g., antibiotic resistance).

**Genome Mapping:**
- Early: microsatellites, RFLPs.
- Modern: long-read sequencing, optical maps, Hi-C technology.

---

## 4. Properties and Structure of Prokaryotic Genomes

| Feature | Description |
|----------|--------------|
| Shape | Circular DNA |
| Size | 0.5–10 Mb |
| Gene Density | High (>85% coding) |
| Organization | Operons (co-transcribed genes) |
| Repeats | Few |
| Introns | Rare |
| Pseudogenes | Few |
| Regulation | Simple promoters/repressors |

**Example:**  
_E. coli_ genome (~4.6 Mb) has ~4,300 genes with minimal non-coding regions.

**Genome Maps:**  
Use concentric circles to show GC content, gene position, origin/terminus of replication, etc.

---

## 5. Eukaryotic Genome Complexity

| Aspect | Eukaryotic Feature |
|--------|--------------------|
| Chromosomes | Linear, multiple per cell |
| Introns/Exons | Present; require splicing |
| Repetitive DNA | High (transposons, microsatellites) |
| Gene Density | Low (~1–2%) |
| Regulation | Complex (enhancers, silencers) |
| Pseudogenes | Common |
| Chromatin | DNA + histones (nucleosomes) |

**Gene Families:** Arise via duplication → subfunctionalization or neofunctionalization.  
Example: Globin gene family.

---

## 6. Reading Frames and Coding Sequences

- DNA is read in triplets (codons).
- Each strand has **3 reading frames** → total of 6 possible.
- **Start codon (ATG)** and **stop codons (TAA, TAG, TGA)** define the open reading frame (ORF).

**Prokaryotes:** Continuous ORFs → easy to predict.  
**Eukaryotes:** Interrupted by introns → complex prediction.

---

## 7. Functional Annotation and Pathway Mapping

**Annotation:** Assigning gene functions using:
- BLAST (homology)
- Pfam / InterPro (domains)
- KEGG / MetaCyc (pathways)

**Pathway Mapping:**
- Maps genes to metabolic pathways.
- Identifies missing enzymes.
- Tools: KEGG Mapper, BlastKOALA.

---

## 8. Gene Duplication and Pseudogenes

### Gene Duplication
Mechanisms:
- Unequal crossing-over
- Retrotransposition
- Whole-genome duplication

Outcomes:
- **Subfunctionalization:** Shared ancestral function.
- **Neofunctionalization:** New function evolves.
- **Redundancy:** Duplicate genes retain same function.

### Pseudogenes
- Non-functional copies due to mutations, deletions, or truncations.
- Can act as molecular fossils or regulatory RNAs.

---

## 9. Genome Variability and Comparative Genomics

- Human–human DNA: ~99.8% identical.
- Coding regions: >99.99% identical.
- Human–chimpanzee: ~98% identical.

**Applications:**
- Identify conserved and variable regions.
- Detect horizontal gene transfer (HGT) in prokaryotes.
- Compare model organisms for functional genomics.

**Tools:** OrthoFinder, Mauve, Pan-genome analysis.

---

## 10. Repeats in the Genome

| Type | Description | Example |
|------|--------------|----------|
| Tandem Repeats | Short sequences repeated head-to-tail | Microsatellites (CACACACA...) |
| Dispersed Repeats | Spread across genome | LINEs, SINEs, Alu |
| Transposons | Mobile DNA elements | DNA transposons, retrotransposons |

**Tools:** RepeatMasker, Tandem Repeats Finder.  
**Significance:** Can drive evolution, cause instability, or complicate genome assembly.

---

## 11. High-Throughput Sequencing Technologies (HTS)

### Major Platforms

| Platform | Read Type | Features |
|-----------|------------|----------|
| Illumina | Short (100–300 bp) | High accuracy, low cost |
| PacBio | Long (>10 kb) | Ideal for structural variants |
| Oxford Nanopore | Ultra-long (up to Mb) | Portable, real-time sequencing |

**Hybrid Assembly:** Combines short and long reads for gapless, accurate genome assemblies.

**Portable Sequencers:**  
- Oxford Nanopore MinION (USB-powered).  
- Used for outbreak surveillance (e.g., Ebola, COVID-19).

---

## 12. Big Data in Biology

**Trends:**
- Biological data doubling every ~7 months.
- Driven by omics studies and affordable sequencing.

**Challenges:**
- Data storage, sharing, and processing.
- Integrating genomics, transcriptomics, proteomics, metabolomics.

**Solutions:**
- Cloud computing
- AI-driven analytics
- High-performance computing (HPC)

---

## 13. Comparison: Prokaryotic vs. Eukaryotic Genomes

| Feature | Prokaryotes | Eukaryotes |
|----------|--------------|-------------|
| Chromosome Shape | Circular | Linear |
| Genome Size | Small (kb–Mb) | Large (Mb–Gb) |
| Gene Density | High (>85%) | Low (~1–2%) |
| Non-coding DNA | Minimal | Extensive |
| Operons | Common | Rare |
| Introns | Absent | Common |
| Repeats | Few | Many |
| Pseudogenes | Rare | Abundant |

---

## 14. Take-Home Points

- **Prokaryotic genomes:** Compact, efficient, and coding-rich.
- **Eukaryotic genomes:** Complex, with regulatory and repetitive elements.
- **Sequencing technologies** have enabled complete genome mapping, function prediction, and evolutionary analysis.

---

## 15. Suggested Reference

🎥 [Prof. Vineet Kumar Sharma – NPTEL Lecture on Genomics](https://www.youtube.com/watch?v=8hQCydGX1gs&list=PLyqSpQzTE6M9F59-Lbh5KzYa_EtaWlbIk&index=3)

---
