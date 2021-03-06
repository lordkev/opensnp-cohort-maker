Create an up to date OpenSNP community cohort from genome-wide genotyping data available on the [OpenSNP platform](www.opensnp.org)

## Dependency

The tools rely on a couple of dependencies.
The versions mentioned were the one used on the last successful run

#### Dependencies in ./bin: 

* bcftools and bgzip (from htslib) (1.5) http://www.htslib.org/download/ (included)
* liftOver (https://genome-store.ucsc.edu/) (free for academics, must be downloaded. Then see the 'Set the dependencies' part)
* unzip (UnZip 6.00 of 20 April 2009, by Debian.) (included)
* gunzip (gzip) 1.6 (included)
* plink (PLINK v1.90b4.5 64-bit) (included)
* vcf-sort (https://vcftools.github.io/license.html) (included)
* rename (The SZABÓ Gergely's version https://github.com/subogero/rename) (included)
* liftMap.py a script that use liftOver (https://genome.sph.umich.edu/wiki/LiftMap.py) (included)

#### Dependencies in ./ref are:

* hg18ToHg19.over.chain.gz  (included)
* human_g1k_v37.fasta and human_g1k_v37.fai  (http://www.internationalgenome.org/data-portal/search?q=%2Bhuman_g1k_v37.fasta) (downloaded if not present in ref at first exxecution)

#### Set the dependencies correctly:

* Either, make a link on each of the tools in the `./bin` directories;
* Or edit the script to specify the location of the tool

## Set the number of cores to use

* Edit the script to set the number of cores available by changing the value of variable `nb_proc` (default is 4)
