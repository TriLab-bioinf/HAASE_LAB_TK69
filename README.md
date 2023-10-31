Suggestions for DOGs overlapping analysis on two stages of spermatogenesis


1. Just with the gene list from the bed files
2. Considering the DOGs length overlapped between two stages, set a cutoff, like 50%, we only consider the genes as overlapped genes when the length overlapped ratio larger than 50% between the twos

Then we can do the following analysis respectively, see which one makes more sense

1. Venn diagram of two DOGs
	Online tool: https://bioinformatics.psb.ugent.be/webtools/Venn/

	R package: Vennerable

2. Functional enrichment of 3 gene sets
	Online tool: http://biit.cs.ut.ee/gprofiler/gost

	R package: clusterProfiler

3. Calculate the ratio of two stage specific DOGs and common DOGs overlapped with piRNA clusters
	Tool: bedtools

4. Statistical test
	DOGs overlapped with piRNA clusters / All DOGs v.s. all piRNA clusters / All peaks

	Statistical method: Fisher's exact test
