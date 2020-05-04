# MSc_TT2020

## Welcome!

*Below is a constantly updating table of resources that I have found useful and think will help to prime you with working with 'high dimensional data'. I will keep updating the table as we go, along, but please add to the list and put comments if you recommend something you have found. This field is constantly developing, and the techniques described are used in a spectrum of disciplines, so you may find answers to your questions on websites not immediately obvious to you!*

- Please sign up for an [Amazon Web Services](https://aws.amazon.com/) account, to access their 'free tier', where you can experiment. Please use your educational email address to join ['AWS Educate'](https://aws.amazon.com/education/awseducate/), so you can obtain free credits for your account, to use more powerful hardware. On AWS, always use 'Europe - London (EU-West-2)'. 

- Please sign up for a [GitHub](github.com) account.

- **Note: Do not install R version 4.0.0! Stay on 3.6.1. Do a quick google to find out why, and we can discuss it if you are interested!**

### Resources

| Topic         | Link(s)       |  Notes |
| :-------------: |:-------------:|:--:|
| **Next-generation sequencing**      | [StatQuest Intro to RNA-Seq](https://www.youtube.com/watch?v=tlf6wYJrwKY&t=410s) | *NGS is getting cheaper every day, and the volume of data being output is huge. It is vital to understand the principles of NGS and to understand the basics of how an 'Illumina Sequencer' works. Find a video/article that works for you and we will talk about it*|
| Learn the command line | [CodeAcademy](https://www.codecademy.com/learn/learn-the-command-line) | *A large amount of pre-processing has to be done to our raw data, before we visualise and analyse it in software such as R or Python. The tools we use to pre-process raw data are designed to be run 'from the command line', specifically, the 'Bash' command line. Codeacademy provides a great primer in how to use some of its functions, which will be essential for when you need to handle the raw data files* |
| Fast-what? | [Fasta/Fastq/SAM](https://bioinformatics.stackexchange.com/questions/14/what-is-the-difference-between-fasta-fastq-and-sam-file-formats) | *An example of a great StackOverflow answer discussing advice about different file formats you will encounter in genetic data* |
| PCA and many other guides      | [PCA StatQuest](https://www.youtube.com/watch?v=FgakZw6K1QQ)      | *StatQuest often provides a good basic introduction to a many statistical concepts. PCA is integral to our work, as we will see later on. I recommend watching other StatQuest videos, and then exploring other videos/online resources if you are interested* |
| Learn Base R  | [Codeacademy](https://www.codecademy.com/courses/learn-r/lessons/introduction-to-r/exercises/why-r) |*This site provides an environment to learn the very basics of R in a short space of time.*|
| Learn R the 'tidy' way | [R4DS](https://r4ds.had.co.nz/index.html)| *Follow this guide's instructions on installing RStudio, the tidyverse package, and use the example datasets it provides to test out some of R's analysis and plotting features. We will use these features with our own data, once we have pre-processed it* |
| StackExchange/Overflow | [StackOverflow](https://stackoverflow.com/) | *I highly encourage getting in the habit of google errors you encounter, as you will find the answer to these errors on sites such as StackOverflow 99% of the time. Googling problems and finding solutions is a valid learning method!* |
|Biostars|[Biostars](https://www.biostars.org/)| *A forum providing discussion topics on many aspects of genetic data analysis.* |
| Bioconductor | [Bioconductor](https://bioconductor.org/) | *Data analysis packages for R are often submitted to 'Bioconductor'; a repository of packages that are required to be maintained and documented to a certain standard, to ensure the public can use the package properly. An example package is 'DESeq2', below. While you are on Bioconductor, check out the [list of top packages](http://www.bioconductor.org/packages/stats/) to see what packages people are using, and think why you might want to use them. They are going to help you!*
| Differential Expression Analysis | [DESeq2 Vignette](https://bioconductor.org/packages/release/bioc/vignettes/DESeq2/inst/doc/DESeq2.html) | *DESeq2 is the often the best R package for differential gene expression analysis. This link will take you to the user guide, which is referred to as a 'vignette' for Bioconductor packages. Start to notice the formats of data that DESeq2 accepts, the importance of how DESeq2 normalises samples, as is plainly explained in the StatQuest video below.* |
| DESeq2 Analysis Workflow | [Vignette](https://www.bioconductor.org/packages/devel/workflows/vignettes/rnaseqGene/inst/doc/rnaseqGene.html) | The title author of DESeq2, Mike Love, also maintains a workflow vignette that you may find easier to interpret in the early stages. This workflow uses an example RNA-seq dataset; 'airway'. This dataset can be installed in R, as a package (google this!). Notice how in the workflow, he refers to the PubMed accession and GEO accession for 'metadata' and 'raw data': These are important sources of information about the experimental details.*|
| Library normalisation | [StatQuest](https://www.youtube.com/watch?v=UFB993xufUU) | *The first video of a series on normalisation. This is one of many resources you will find on the internet about the importance of normalisation in data analysis. You may find that watching the [FPKM/TPM video](https://www.youtube.com/watch?v=TTUrtCY2k-w) alongside helps.*|

### Papers

*Here are some of the papers from our lab that concern RNA-seq data. Make a note of the methods used to produce and analyse the data, and think of the challenges that may be present in analysing it. We will be using these datasets by first replicating the analysis, then looking to compare independent studies (GBA & LRRK2 - Tara), or investigate splicing (LRRK2 transcriptome-wide - Eugenio, LRRK2 specifically - Guusje*

  - [Single-Cell Sequencing of iPSC-Dopamine Neurons Reconstructs Disease Progression and Identifies HDAC4 as a Regulator of Parkinson Cell Phenotypes.](https://www.ncbi.nlm.nih.gov/pubmed/30503143)
  - [RNA sequencing reveals MMP2 and TGFB1 downregulation in LRRK2 G2019S Parkinson's iPSC-derived astrocytes.](https://www.ncbi.nlm.nih.gov/pubmed/31085228)
  - [Transcriptomic profiling of purified patient-derived dopamine neurons identifies convergent perturbations and therapeutics for Parkinson’s disease.](https://academic.oup.com/hmg/article/26/3/552/2917762)
  - [Cellular α-synuclein pathology is associated with bioenergetic dysfunction in Parkinson’s iPSC-derived dopamine neurons](https://academic.oup.com/hmg/article/28/12/2001/5315478)
  
### Packages/commands often used
```
- ls, cd, mv, cp, rm, htop, ssh, screen, cut, sort, uniq, >, |, for i in *, parallel, echo
- BioMaRt
- Tidyverse (ggplot2, dplyr, tidyr...)
- prcomp
- kallisto
- tximport
- deseq2
- fastqc
- STAR
- multiqc
- trim_galore
```

*This is growing list of packages/commands that are very useful*
