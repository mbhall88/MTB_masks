## Genomic Masks for *Mycobacterium tuberculosis*

### `modlin.bed`

This mask contains all of the blind spots from [Modlin *et al.*][modlin]. Note: these are **Illumina** blind spots; whether they also apply to other sequencing technologies is yet to be determined.

### `marin-PMapK50E4.bed`

Taken from [Marin *et al.*][marin] (Additional File 20). 

> We identified repetitive regions in H37Rv and evaluated their relationship with low EBR using the pileup mappability metric (Section 4). Pileup mappability scores range from 0 to 1, where 1 represents a genomic position where all overlapping sequence K-mers are unique in the genome of interest within a similarity threshold of E mismatches. We calculated pileup mappability conservatively with a K-mer size of 50 base pairs and up to 4 mismatches (P-Map-K50E4)

### `marin-rlc.bed`

Taken from [Marin *et al.*][marin] (Additional File 13)

> the refined low confidence regions (RLC) of the Mtb reference genome as the union of A) The 30 false positive hot spot regions (gene and intergenic) identified (65 kb), B) poorly recalled genomic regions as identified by EBR (EBR < 0.9, 142 kb), and C) regions with frequently ambiguously defined ground truths (16 kb)

### `marin-conservative.bed`

This is the union of `marin-rlc.bed` and `marin-PMapK50E4.bed`.

### `marin-modlin.bed`

This is the union of `marin-conservative.bed` and `modlin.bed`

[marin]: https://doi.org/10.1093/bioinformatics/btac023
[modlin]: https://doi.org/10.1099/mgen.0.000465