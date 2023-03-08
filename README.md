# Tn-seq correction

Transposon insertion sequencing (Tn-seq) is a sensitive and reliable method used to discover quantitative genetic interactions of transposons in microorganisms [1]. A transposon insertion library is created, followed by sequencing to calculate changes in frequency for all insertion mutants. Using these changes, a score is calculated to indicate if an inserted mutation has a positive or negative effect on bacterial growth.

However, due to the circular nature of the bacterial genome, nucleotides near the origin of replication (ORI) may be sequenced more frequently than other nucleotides during replication, resulting in bias in the scores.

The objective of this project is to address this bias. We accomplished this by first transforming genomic coordinates into radians to formalize the problem more accurately. Then, we fitted models using linear regression and conducted a series of preliminary operations on the data, such as dividing the genome into windows. Through these methods, we successfully eliminated the bias.

[1] van Opijnen T, Bodi KL, Camilli A. Tn-seq: high-throughput parallel sequencing for fitness and genetic interaction studies in microorganisms. Nat Methods. 2009 Oct;6(10):767-72. doi: 10.1038/nmeth.1377. Epub 2009 Sep 20. PMID: 19767758; PMCID: PMC2957483.
