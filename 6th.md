**Long Read Sequencing and Linked Read Sequencing – Detailed Notes**

***

**1. Introduction & Recap**
- Long read sequencing is a post-Illumina next-gen technology, providing much longer reads than traditional first (Sanger) and second gen (Illumina) approaches.
- DNA and RNA (converted to DNA) can both be sequenced.
- Earlier technologies (Sanger: long but low throughput, low errors; Illumina: short but high throughput, cheap) have limitations for assembling large or complex genomes.

***

**2. Second Generation Sequencing Technologies (Review)**
- *Pyrosequencing*: Each nucleotide addition releases pyrophosphate, converted to ATP, detected by luciferase-generated light. Very parallel, can handle long reads, but expensive due to enzyme/reagent use.
- *Ion Torrent*: Each base addition releases a proton, changing pH detected by sensors (non-optical). Fast, but suffers with homopolymers and reagent cost.
- *Illumina*: Bridge amplification, sequencing by synthesis using fluorescent tags. Massively parallel, error rates low, but read lengths are short (e.g., 75–300 bp).

***

**3. Third Generation Sequencing Technologies**
- *General Advantages*:
  - No amplification needed (single-molecule sequencing).
  - Provides extremely long reads (thousands to millions of bases).
  - Faster library preparation, real-time data acquisition.
  - Initially higher error rates, but error correction is feasible (consensus from multiple reads, hybrid assembly).
- *Major Platforms*:
  - **PacBio (SMRT):** Long reads, useful for assembling repeat-rich regions.
  - **Oxford Nanopore Technology (ONT):** Key focus of the video.

***

**4. Nanopore Sequencing (Oxford Nanopore)**
- A single-stranded DNA/RNA molecule passes through a protein nanopore embedded in a synthetic membrane.
- As each different nucleotide passes through, it disrupts ionic current in a characteristic way—this change is detected electronically and converted into sequence data.
- *Features*:
  - Real-time data streaming and analysis.
  - No need for expensive PCR enzymes or nucleotide consumables.
  - Devices: **MinION** (USB-sized for field use, up to 30GB data), **GridION**/**PromethION** (higher throughput for labs).
  - Error rate currently ~10%, decreasing with new developments; multiple reads help correct errors.
- Processes:
  - DNA is converted to single strand (via helicase).
  - Distinct current disruptions for A/T/G/C allow identification of each nucleotide.
  - Data is base-called and assembled, often with overlapping reads for contiguity.

***

**5. Linked Read Sequencing (10x Genomics Chromium)**
- DNA is fragmented and barcoded individually using microfluidics; fragments from the same molecule get the same barcode.
- Short reads sequenced (Illumina) are grouped computationally by barcode, reconstructing much longer contiguous sequences ("linked reads").
- *Features*:
  - Long-range information from short-read instruments.
  - Requires barcoding, microfluidics; methods evolving due to platform changes in the field.

***

**6. Comparison Table**

| Technology                  | Read Length         | Amplification | Error Rate   | Instrument      | Cost         | Real-Time    |
|-----------------------------|--------------------|--------------|-------------|-----------------|--------------|--------------|
| Sanger                      | 500–800 bp         | Yes          | Very Low    | Capillary       | High/base    | No           |
| Illumina                    | 75–300 bp          | Yes          | Low         | Flow cell       | Low/base     | No           |
| Pyrosequencing/Ion Torrent  | 100–1000 bp        | Yes          | Moderate    | Optical/Electro | Moderate     | No           |
| Nanopore (ONT)              | 1 kb–>1 Mb+        | No           | Moderate    | MinION etc      | Affordable   | Yes          |
| Linked reads (10X Chromium) | Reconstructed kbs  | Yes          | Low (hybrid)| Illumina+10X    | Moderate     | No           |

***

**7. Applications & Considerations**
- Long reads solve challenges with repetitive regions, structural variations, gap closure, and haplotype phasing.
- Nanopore sequencing used for rapid diagnostics, metagenomics, remote field science.
- Linked reads allow assembly of complex genomes with limited resources by reconstructing context from short reads.

***

**8. Conclusion**
- Long read sequencing (Nanopore, PacBio) and linked read technologies (10x Chromium) represent next-generation solutions to biological data assembly.
- They offer new possibilities for accuracy, contiguity, and accessibility, now central to modern genomics and transcriptomics workflows.
### references
[1](https://www.youtube.com/watch?v=6Dv0kH1565g&list=PLyqSpQzTE6M9F59-Lbh5KzYa_EtaWlbIk&index=6)

