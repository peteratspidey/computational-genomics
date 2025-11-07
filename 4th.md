# **Databases and Web Resources to Store and Access Biological Data – Detailed Notes**

***

**1. Introduction to Biological Databases**
- **Database:** Structured collection of data for storage, retrieval, and management; essential for organizing vast quantities of biological information generated worldwide.
- **Database Management System (DBMS):** Software for database organization (Oracle, MySQL, Microsoft Access, FoxPro). Enables structured queries (SQL) for fast data access, curation, and security.

***

**2. Importance of Data Organization**
- Centralized storage allows global access, collaboration, and re-use.
- Data is standardized—ensures uniform submission and retrieval across platforms.
- Databases verify, validate, and curate submitted information.

***

**3. Querying and Retrieval**
- Data retrieval using structured query languages (e.g., SQL).
- Boolean operators (*AND, OR, NOT*) refine search results (e.g., searching for protein kinase AND human).
- Multiple users can access and download data simultaneously (FTP for large datasets).

***

**4. Key Database Categories & Examples**
- **Nucleotide Sequence Databases:** 
  - NCBI GenBank (US), EMBL (Europe), DDBJ (Japan).
  - Store DNA/RNA sequences and annotation.
- **Protein Sequence Databases:**
  - NCBI, UniProtKB (Swiss-Prot, TrEMBL), Expasy.
  - Raw, curated, and predicted protein sequences.
- **Structural Databases:**
  - Protein Data Bank (PDB): 3D protein structures via X-ray, NMR, Cryo-EM.
- **Genome Browsers:**
  - UCSC Genome Browser: Visualization, annotation, comparative genomics.
  - Ensembl: Genome data and tools for a broad range of species.
- **Literature Databases:**
  - PubMed: Indexed scientific publications, abstracts, citations.
- **Metabolic, Pathway, and Metabolomic Databases:**
  - KEGG: Maps genes/proteins to biochemical pathways (glycolysis, TCA, carbon metabolism).
  - HMDB (Human Metabolome Database): Comprehensive metabolite data.

***

**5. Using Key Resources**
- **NCBI Portal:**
  - Comprehensive access to nucleotide, protein, gene, assembly, literature, and more.
  - Provides tools for basic analysis (primer checks, ORF finder, pattern search).
  - Requires login/registration for data submission and extended features.
  - Submission: Data must conform to standards for acceptance, curation, and future public access.
- **Search Examples:**
  - Search terms can be refined by species, annotation keywords, authors (in literature), or by Boolean combinations.
  - Search result organization: summary tables, download options (FASTA, other formats), and advanced filters.
- **Data Download and Submission:**
  - Individual, batch, or FTP-based (for large-scale data).
  - Unique accession numbers provided for submitted records.

***

**6. Genome Project and Status Databases**
- **GOLD (Genomes Online Database):** 
  - Tracks global genome and metagenome sequencing projects (completed, ongoing), with statistics and details by organism and environment.

***

**7. Special Topics**
- **Non-redundant Databases:** 
  - Remove duplicate sequences to optimize storage/search (e.g., NCBI NR for BLAST).
- **Data Security:** 
  - Password-protection, access control for sensitive or pre-publication data.
- **Integration:** 
  - Many databases are interlinked (e.g., NCBI ↔ EBI ↔ DDBJ); allows cross-referencing.
- **Functional Tools Embedded:**  
  - Genome browsers with BLAT/BLAST for sequence search and alignment.

***

**8. Pathway and Functional Integration**
- KEGG: Detailed pathway maps, gene/protein functional assignments, presence/absence mapping.
- Ability to upload custom data or compare genomes for pathway completeness and conservation.

***

**9. Metabolomics**
- HMDB: Extensive data on human metabolites, their chemical properties, structures, and related genes/enzymes.
- Increasing importance as systems biology investigates final products of metabolic processes.

***

**Summary Table: Key Bioinformatics Databases**

| Type                  | Example(s)                   | Major Focus                      |
|-----------------------|------------------------------|----------------------------------|
| Nucleotide sequence   | NCBI GenBank, EMBL, DDBJ     | DNA/RNA sequences                |
| Protein sequence      | UniProtKB, Expasy, TrEMBL    | Protein sequences, annotation    |
| Structural            | PDB                          | Protein 3D structures            |
| Genome browsers       | UCSC, Ensembl                | Visualization, comparative genomics|
| Literature            | PubMed                       | Scientific literature            |
| Metabolic/pathway     | KEGG                         | Pathways, functional annotation  |
| Metabolomic           | HMDB                         | Metabolite data                  |
| Project tracking      | GOLD                         | Genome, metagenome project status|

***

**10. Takeaway Points**
- Biological databases are foundational for modern research and collaboration.
- Knowledge of key resources, proper querying, and data management is essential for computational genomics, proteomics, and systems biology.
- Database skills (e.g., SQL, data curation, data integration) are highly valuable for bioinformatics professionals.
### references
[1](https://www.youtube.com/watch?v=hT0NVPlJdZs&list=PLyqSpQzTE6M9F59-Lbh5KzYa_EtaWlbIk&index=4)

