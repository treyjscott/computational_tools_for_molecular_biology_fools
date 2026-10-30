# Alignments

Alignments are hypotheses. They are a guess about which residues are derived from a common ancestor. What this means practically, is that you should have some healthy skepticism about any alignment you make. The best way to deal with this is to explicitly [account for alignment uncertainty](https://academic.oup.com/sysbio/article-abstract/68/1/117/4996308), but this is not practical in many cases. Here, I will describe some general practices for making and checking a single alingment to use in gene trees or other analyses.

Alignments can be made from DNA or amino acid sequences (they can also be made at the protein structure level but that is a topic for another day). There are many programs that will generate alignments and making better alignment tools is an active area of research. For many purposes, MAFFT works well so I will start with that program.

Once you have MAFFT [installed](), you can generate an alignment. If you do not have sequences of your own you can use the some_proteins.faa file in the [data](https://github.com/treyjscott/computational_tools_for_molecular_biology_fools/tree/main/data) directory.

