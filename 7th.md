# **Long Read Sequencing and Linked Read Sequencing – Part 02 (PacBio SMRT and TELL-Seq) – Detailed Notes**

***

**1. Review of Previous Concepts**
- Short-read sequencing (Illumina): High throughput, cost-effective, but short reads (≤300 bp) make assembly challenging, especially for complex genomes.
- Linked-read sequencing (10x Genomics, Chromium): DNA fragments are barcoded, sequenced on Illumina, reconstructed computationally to enable longer effective reads and better assembly from short-read data.

***

**2. Recap of Nanopore Sequencing**
- DNA/RNA passes through a nanopore; ionic current change per base creates the profile for base identification.
- Key features: real-time, field-portable (MinION), handles long fragments (10–100 kb or more), but higher error rate than Illumina.
- Hybrid assemblies (Nanopore + Illumina) increase sequence quality.

***

**3. PacBio SMRT (Single Molecule Real Time) Sequencing**
- **Technology:**
  - Uses a “SMRTbell” template: DNA with hairpin adapters at both ends.
  - The single circular DNA molecule is immobilized in a Zero-Mode Waveguide (ZMW) well.
  - DNA polymerase synthesizes, incorporating fluorescently labeled nucleotides.
  - Each incorporation yields a fluorescence signal detected in real time.
- **Advantages:**
  - Produces very long reads (average 10–20 kb, sometimes >100 kb).
  - Suitable for large, complex genomes and full-length transcriptome sequencing—excellent for capturing alternative splicing and isoforms.
  - Captures DNA modifications (e.g., methylation).
  - More uniform genome coverage (less bias from library prep).
- **Drawbacks:**
  - Higher instrument and library preparation costs than ONT Nanopore.
  - Still has moderate error rates, but errors decrease with improved chemistry and by deep or hybrid sequencing.

***

**4. Comparative Overview: PacBio vs. Nanopore**
| Feature         | PacBio SMRT         | Oxford Nanopore       |
|-----------------|---------------------|-----------------------|
| Read Length     | Very long (10–100 kb, occasional >100 kb) | Very long (10–100 kb or more) |
| Signal/Input    | Fluorescent + polymerase | Ionic + nanopore     |
| Cost            | Higher (instrument, reagents) | Lower (field deployable) |
| Prep Time       | Moderate             | Short                 |
| Use Cases       | Genome assembly, transcriptomics, epigenomics | Field/rapid sequencing, assembly, diagnostics |

***

**5. New Linked Read Sequencing by Illumina (TELL-Seq)**
- **TELL-Seq:**  
  - Based on transposase-linked long-read technology.
  - DNA is fragmented, captured and barcoded with beads, then amplified.
  - Enables read reconstruction from very low DNA input (0.1–5 ng).
  - Quick workflow (results within a few hours).
  - Uses Illumina sequencers with a specific assembler (Turing assembler).
  - Especially useful for small and medium genomes and ultra-low sample amounts (tractable for rare or precious samples).

***

**6. Practical Workflow Example: Metagenomics**
- Steps:
  1. Sample Collection and Storage (–20°C for short, –80°C for long term).
  2. DNA extraction with specialized kits.
  3. Library preparation depending on sequencing platform and project scale (e.g., NEXtera for small DNA, TruSeq for larger DNA).
  4. Indexing for multiplexing samples on a single flow cell (up to instrument capacity, e.g., 120 GB per run).
  5. Sequencing (library is run according to selected protocols and flow cell type).
  6. Data Analysis: Assembly, annotation, taxonomic/functional profiling.

***

**7. Applications & Considerations**
- PacBio and ONT are “gold standards” for long read sequencing—central to reference-quality assemblies, full-length transcriptomics, epigenetics, and metagenomics.
- TELL-Seq and other linked-read methods allow high contiguity assembly even from minimal samples on mainstream sequencers.
- Choice of platform depends on genome size, complexity, sample availability, and budget.

***

**8. Conclusion**
- Technological advances in both long-read and linked-read sequencing democratize genomics, making high-quality assemblies possible even for non-model organisms and environmental communities.
- Hybrid approaches (combining short and long reads) optimize accuracy and contiguity for modern genomic projects.
### references
[1](https://www.youtube.com/watch?v=SWYGPYuvvy0&list=PLyqSpQzTE6M9F59-Lbh5KzYa_EtaWlbIk&index=7)
