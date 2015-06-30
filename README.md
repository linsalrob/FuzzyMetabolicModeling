Fuzzy Metabolic Modeling
========================

This is code from Rob Edwards' bioinformatics group about fuzzy metabolic modeling and their implementations to solve challenges in microbial genomics and metagenomics

We want metabolic networks to answer three questions:

# 1. Can this bacteria grow on that media?

This is trivial, because this is what FBA is designed for. Can we generate biomass on a particular growth substrate?

The main problem that we have with this is largely incorrect annotations of the genes in the genomes (something we're fixing with the metabolic analysis project). Secondarily is whether we miss a gene that should be there, for example because we only have a partial genome. From *Citrobacter* it seems that most of our issues were because the gene was incorrectly annotated, not that it was missing in the sequences.

# 2. What substrates are a metagenome using?

This is a lot more complex because we know we don't have all the genes in the model. We need a new way to think about how to model the network given that it is known to be incomplete.

# 3. If we observe a peturbation in metabolites, which gene(s) have been affected?

This is the viral dark matter goal of overexpressing some genes and seeing what happens to the cellular network.

