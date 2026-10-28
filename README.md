# DNA/Protein Sequence Analysis Using BLAST

**CodeAlpha Bioinformatics Internship – Task 1**

> **Project status:** Setup complete. BLAST analysis, results table, screenshots and report are **to be added** after I run the search myself. No results are claimed below until they are filled in.

## Internship Information
| | |
|---|---|
| Organization | CodeAlpha |
| Domain | Bioinformatics |
| Task | Task 1 – DNA/Protein Sequence Analysis |
| Author | Vikash Raj Patel |
| Program | Integrated M.Tech in Artificial Intelligence and Bioinformatics, VIT Bhopal |

## Project Overview
This project downloads a well-studied protein sequence from UniProt, searches for similar sequences with NCBI Protein BLAST (`blastp`), and interprets the alignment statistics (percentage identity, positives, alignment score, E-value, query coverage) to understand how sequence similarity can suggest an evolutionary relationship (homology).

## Aim and Objectives
**Aim:** To identify homologous sequences of human cytochrome c using BLAST and interpret the results.

**Objectives**
- Retrieve a protein sequence in FASTA format from UniProt.
- Run `blastp` against an NCBI protein database.
- Record identity, similarity, alignment score, E-value and query coverage.
- Interpret the results biologically and explain the difference between similarity and homology.
- Prepare a 2–3 page report with screenshots.

## Biological Sequence Selected
| Item | Detail |
|---|---|
| Protein | Cytochrome c |
| Gene | *CYCS* |
| Organism | *Homo sapiens* (human) |
| UniProtKB accession | **P99999** (entry name `CYC_HUMAN`) |
| Length | 105 amino acids |
| Source | https://www.uniprot.org/uniprotkb/P99999 |

**Function (summary):** Cytochrome c is a small heme-containing protein in the mitochondrial intermembrane space. It carries electrons from Complex III to Complex IV in the electron transport chain, and when released into the cytosol it helps trigger apoptosis by activating Apaf-1 and caspase-9.

**Why this protein?** It is short, well studied, highly conserved across species, and gives clear, easy-to-interpret BLAST results for a beginner.

The sequence is stored in [`protein_sequence.fasta`](protein_sequence.fasta). Please re-download it from UniProt (*Download → FASTA*) and confirm it matches before final submission.

## Tools and Technologies
- UniProt (sequence retrieval)
- NCBI Protein BLAST – `blastp`
- FASTA format
- GitHub, Google Drive, Microsoft Word (report)

## Methodology
1. Open UniProt entry **P99999** and download the sequence in FASTA format.
2. Save it as `protein_sequence.fasta`.
3. Open NCBI Protein BLAST and paste the FASTA sequence as the query.
4. Select program `blastp` (protein query vs. protein database) and keep default settings.
5. Run the search and review the top hits.
6. Open individual alignments and record the statistics.
7. Save results in `BLAST_Results.txt` and capture screenshots.

Database used: `[to be filled after running BLAST]`
Date of search: `[to be filled]`

## BLAST Parameters Analyzed
| Parameter | Meaning |
|---|---|
| Percentage identity | Share of aligned positions with exactly the same amino acid |
| Positives (similarity) | Share of aligned positions that are identical or chemically similar |
| Alignment (bit) score | Alignment quality; higher means a better match |
| E-value | Number of matches this good expected by chance; lower is more significant |
| Query coverage | Share of the query sequence included in the alignment |
| Gaps | Insertions/deletions introduced to align the sequences |

## Results Summary
*To be completed with real BLAST output. Do not fill with estimated values.*

| Parameter | Observed Value | Interpretation |
|---|---|---|
| Query protein | Cytochrome c (P99999) | Sequence analyzed |
| Matching protein | _pending_ | Matching database entry |
| Organism | _pending_ | Biological source |
| Percentage identity | _pending_ | Identical aligned residues |
| Percentage positives | _pending_ | Similar amino acid substitutions |
| Alignment score | _pending_ | Alignment quality |
| E-value | _pending_ | Statistical significance |
| Query coverage | _pending_ | Fraction of query covered |

## Biological Interpretation
*To be written after results are obtained.* It will discuss what the identity and E-value suggest about conservation of cytochrome c, and note that high similarity supports (but does not by itself prove) homology.

## Repository Structure
```
CodeAlpha_DNA_Protein_Sequence_Analysis/
├── README.md                       # Project overview (this file)
├── protein_sequence.fasta          # Query sequence, UniProt P99999
├── BLAST_Results.txt               # Recorded BLAST output and statistics
├── Sequence_Analysis_Report.docx   # Editable 2–3 page report (to be added)
├── Sequence_Analysis_Report.pdf    # Final PDF report (to be added)
├── screenshots/                    # Genuine workflow screenshots (01–05)
└── references.txt                  # Databases, tools and citations
```

## How to View the Results
Open `BLAST_Results.txt` for the data, `screenshots/` for the workflow images, and the report PDF for the full discussion.

## References and Official Links
- UniProt: https://www.uniprot.org/
- UniProtKB P99999: https://www.uniprot.org/uniprotkb/P99999
- NCBI: https://www.ncbi.nlm.nih.gov/
- NCBI Protein BLAST: https://blast.ncbi.nlm.nih.gov/Blast.cgi?PAGE=Proteins

See [`references.txt`](references.txt) for the full list.

## Author
**Vikash Raj Patel**
Integrated M.Tech in Artificial Intelligence and Bioinformatics, VIT Bhopal
