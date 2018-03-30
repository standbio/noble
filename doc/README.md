# Noble Trios: simulated pedigrees for benchmarking *de novo* variant discovery methods

Daniel S. Standage, 2018  
https://osf.io/anr56/

[![Docker image status at quay.io](https://quay.io/repository/standage/noble/status "Docker ready")](https://quay.io/repository/standage/noble)


## Motivation

Modeling genome sequences realistically is incredibly complicated, and most simulations are gross oversimplifications of many features observed in real data.
Nevertheless, there is tremendous value, espcially while developing new methods, in frequently evaluating performance on a data set where the "correct" answers are known.
While the true test of a method is its accuracy with real sequence data, experience demonstrates that even trivially small simulated data sets can reveal bugs in software and bring erroneous assumptions to the fore.
Deliberately small data sets can also be processed in much less time with fewer computational resources, enabling continuous testing strategies not feasible with large data sets.

## Availability

**Noble** is a collection of simulated pedigrees created for assessing the performance of *de novo* variant discovery methods.
Each trio is derived from a randomly generated genome sequence with a septanucleotide composition equivalent to that of the human genome.
From this "reference" sequence, shared (inherited) and unique (*de novo*) genomic variants are simulated for three hypothetical individuals: a mother, father, and child.
For each trio this data set furnishes a Fastq file containing simulated 2x100bp paired-end Illumina reads providing 30x coverage of each sample, as well as a VCF file annotating the locations of the shared and unique variants.

Sequence data and variant annotations can be obtained anonymously from the Open Science Framework at https://osf.io/anr56/.
Full disclosure of the pipeline used to produce the data set is available at https://github.com/standage/noble.


## Meet the Nobles

**Noble** includes four simulated pedigrees, associated with genomes ranging in size from 2.5 Mbp to 2.5 Gbp.
Each pedigree includes 3 individuals: a mother, a father, and a proband.
Each pedigree also includes variants shared between some or all individuals (representing inherited mutation) as well as variants unique to the proband (representing *de novo* germline mutation).


|  Trio name  |  Genome size (Mbp)  |  # Shared variants  |  # Unique (*de novo* in proband) variants  |
|-------------|--------------------:|--------------------:|-------------------------------------------:|
|  helium     |           2.5       |               100   |                                       5    |
|  neon       |          25.0       |               200   |                                      10    |
|  argon      |         250.0       |               300   |                                      20    |
|  krypton    |        2500.0       |               750   |                                      60    |
