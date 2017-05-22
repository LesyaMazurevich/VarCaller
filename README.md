# VarCaller

VarCaller is the worlds most lightweight varaiant caller!

It is a wrapper that uses samtools and bcftools to call variants.

Input is processed as one or two reads and is mapped to the reference (a fasta or a genbank file, more support for other file type coming) via BWA mem.  From there variants are called using samtools and bcftools. 

Current dependencies: Python (version 2.7), BioPython, samtools (version 1.4), bcftools (version 1.2), bwa (version 0.7.15)
