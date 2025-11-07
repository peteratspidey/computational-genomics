# **First and Second Generation Sequencing Technologies – Detailed Notes**

***

## **1. Principle of Sequencing**
- **Goal:** Determine nucleotide identity and order for DNA (mainly) or RNA at each position.
- **Base terminology:** Read length, fragments, paired-end/single-end, coverage, contig, scaffold, draft vs. complete genome.

***

## **2. Historical Perspective & Evolution**
- **First Generation Sequencing:**
  - *Sanger Sequencing (Chain Termination)* – Developed 1977.
    - Key stages: DNA template, primer, DNA polymerase, dNTPs + chain-terminating ddNTPs (di-deoxy).
    - Each ddNTP prevents further extension, producing a ladder of fragments.
    - Fragments separated by capillary electrophoresis, detected by fluorescent labeling.
    - Produces long reads (up to 800 bp), low error rates, accurate but low throughput.
    - Suitable for small genomes or molecular marker identification.
  - *Maxam-Gilbert Sequencing* – Historical chemical degradation method, less commonly used.

- **Second Generation (Next-Generation) Sequencing:**
  - *Pyrosequencing, 454/Roche* – High cost, ultimately less sustained use.
  - *SOLiD, Ion Torrent* – Competing, but Illumina became standard.
  - *Illumina Sequencing (Sequencing by Synthesis):*
    - Library construction: DNA fragmentation and adapter ligation.
    - Bridge amplification on a flow cell—creates clusters.
    - Each cluster contains many copies of the same DNA piece.
    - Sequencing via fluorescently labeled reversible terminator nucleotides (all four blocked).
    - Each nucleotide imaged in cycles—producing short, massively parallel reads (75–300 bp).
    - Output in gigabases–terabases per run at very low cost per base.
    - Allows multiplexing via barcoding.
    - Limitations: Short read length, computational assembly required, not ideal for a single piece.

***

## **3. Shotgun Sequencing and Assembly**
- **Shotgun:** Random DNA fragmentation followed by sequencing; fragments then assembled computationally into drafts or complete genomes.
- **Contigs:** Overlapping reads form longer sequences.
- **Scaffold:** Ordered, oriented set of contigs, may contain gaps.
- **Coverage:** Critical—aim for enough redundancy to confidently assemble genome.  
  Formula:  
  $$
  \text{Coverage} = \frac{n \times L}{G}
  $$
  where $$ n $$=number of reads, $$ L $$=read length, $$ G $$=genome size.

***

## **4. Single-End vs. Paired-End Reads**
- **Single-End:** Sequence from one end—simpler, less information.
- **Paired-End:** Sequence both ends of DNA fragments; better assembly, detect repeats/adjacencies.

***

## **5. Library Preparation and Amplification**
- **First Gen:** Cloning into vectors, bacterial amplification for sufficient material.
- **Second Gen:** In vitro amplification (bridge amplification on flow cell, not cloning/bacterial cells).

***

## **6. Technical Differences and Advancements**
| Parameter                | Sanger (1st Gen)          | Illumina (2nd Gen)            |
|--------------------------|---------------------------|-------------------------------|
| Read length              | 500–800 bp                | 75–300 bp                     |
| Throughput               | Low                       | Massive (Gb–Tb/run)           |
| Error rate               | Very low                  | Low                           |
| Cost                     | High per base             | Very low per base             |
| Application              | Small targets, validation | Whole genome, large projects  |
| Single-piece sequencing  | Yes                       | Not cost-effective            |
| PCR/Amplification        | Bacterial cloning         | Bridge amp on flow cell       |
| Assembly challenge       | Low                       | High (short reads)            |

***

## **7. Sequencing Workflow Overview**
- **Sanger Example:**
  - DNA + primer + polymerase + dNTPs/ddNTPs → chain-terminated fragments
  - Capillary electrophoresis → color-separated "read"
- **Illumina Example:**
  - DNA fragmentation + adapter ligation
  - Bridge amplification (many clusters)
  - Sequencing cycles: incorporation, imaging, blocker removal, next cycle
  - Millions of reads obtained in parallel

***

## **8. Instrumentation**
- Advance in sequencer design: moving from rooms full of Sanger sequencers (Human Genome Project) to single machines (Roche, Illumina) to ever smaller, higher throughput platforms (MySeq, NextSeq, HiSeq, NovaSeq).

***

## **9. Applications & Limitations**
- Sanger: Still used for targeted gene/molecular marker validation.
- Illumina: Dominant for genomics, transcriptomics, metagenomics, high-throughput data.
- Challenges: Short read assembly (Illumina), cost-per-sample (Sanger), computational needs.

***

## **10. Takeaway Points**
- First and second generation sequencing revolutionized biology with different trade-offs.
- Illumina enables data-driven genomics, while Sanger’s accuracy preserves its niche in targeted and validation assays.
- Newer (third/fourth generation) long-read technologies further resolve genome complexities, but Sanger and Illumina remain pillars for basics and big-data, respectively.
### references
[1](https://www.youtube.com/watch?v=sCPFiK0ma7o&list=PLyqSpQzTE6M9F59-Lbh5KzYa_EtaWlbIk&index=5)
