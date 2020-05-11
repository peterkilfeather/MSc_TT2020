# MSc_TT2020

## Welcome!

*Here is a constantly updating set of resources that I have found useful and think will help to prime you with working with 'high dimensional data'. I will keep updating the table as you go along, but please add to the list and put your own notes in if you recommend something you have found. This field is constantly developing, and the techniques described are used in a spectrum of disciplines, so you may find answers to your questions on websites not immediately obvious to you!*

- Please sign up for an [Amazon Web Services](https://aws.amazon.com/) account using your educational email address, to access their 'free tier', where you can experiment. Please then join ['AWS Educate'](https://aws.amazon.com/education/awseducate/), so you can obtain free credits for your account, to use more powerful hardware. On AWS, always use 'Europe - London (EU-West-2)'. Set up a t2.micro (free-tier) 'EC2' instance, with 30GB (free-tier) of 'EBS' storage. If this is confusing, I agree! Google helps a lot.

- Please sign up for a [GitHub](github.com) account.

- **Note: Do not install R version 4.0.0! Stay on 3.6.1. Do a quick google to find out why, and we can discuss it if you are interested!**

## Resources

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
| DESeq2 Analysis Workflow | [Vignette](https://www.bioconductor.org/packages/devel/workflows/vignettes/rnaseqGene/inst/doc/rnaseqGene.html) | *The title author of DESeq2, Mike Love, also maintains a workflow vignette that you may find easier to interpret in the early stages. This workflow uses an example RNA-seq dataset; 'airway'. This dataset can be installed in R, as a package (google this!). Notice how in the workflow, he refers to the PubMed accession and GEO accession for 'metadata' and 'raw data': These are important sources of information about the experimental details.*|
| Library normalisation | [StatQuest](https://www.youtube.com/watch?v=UFB993xufUU) | *The first video of a series on normalisation. This is one of many resources you will find on the internet about the importance of normalisation in data analysis. You may find that watching the [FPKM/TPM video](https://www.youtube.com/watch?v=TTUrtCY2k-w) alongside helps.*|
| Visualising data with Shiny | [Shiny Gallery](https://shiny.rstudio.com/gallery/) | *Getting familiar with different ways of plotting data helps you understand your data better and share your findings. R provides 'Shiny', a service whereby your analysis results can be input into a great-looking website that you can share. Check out the gallery and then google some examples of RNA-seq analyses that are in R Shiny format.*|

## Papers

*Here are some of the papers from our lab that concern RNA-seq data. Make a note of the methods used to produce and analyse the data, and think of the challenges that may be present in analysing it. We will be using these datasets by first replicating the analysis, then looking to compare independent studies (GBA & LRRK2 - Tara), or investigate splicing (LRRK2 transcriptome-wide - Eugenio, LRRK2 specifically - Guusje*

  - [Single-Cell Sequencing of iPSC-Dopamine Neurons Reconstructs Disease Progression and Identifies HDAC4 as a Regulator of Parkinson Cell Phenotypes.](https://www.ncbi.nlm.nih.gov/pubmed/30503143)
  - [RNA sequencing reveals MMP2 and TGFB1 downregulation in LRRK2 G2019S Parkinson's iPSC-derived astrocytes.](https://www.ncbi.nlm.nih.gov/pubmed/31085228)
  - [An integrated transcriptomics and proteomics analysis reveals functional endocytic dysregulation caused by mutations in LRRK2](https://www.sciencedirect.com/science/article/pii/S0969996119300968?via%3Dihub)
  - [Transcriptomic profiling of purified patient-derived dopamine neurons identifies convergent perturbations and therapeutics for Parkinson’s disease.](https://academic.oup.com/hmg/article/26/3/552/2917762)
  - [Cellular α-synuclein pathology is associated with bioenergetic dysfunction in Parkinson’s iPSC-derived dopamine neurons](https://academic.oup.com/hmg/article/28/12/2001/5315478)
  
*Analysis package papers/examples of interesting analysis methods*
- [Annotation-free quantification of RNA splicing using LeafCutter](https://www.nature.com/articles/s41588-017-0004-9)
- [Integrative transcriptome analyses of the aging brain implicate altered splicing in Alzheimer’s disease susceptibility](https://www.nature.com/articles/s41588-018-0238-1)

## Packages/commands often used

*This is growing list of packages/commands that I use very often*

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
- Cluster Window Manager for Google Chrome: A Godsend

```

## Week 1 Task list - Updated Wednesday

- [x] Learn command line essentials (cd, ls, mv, cp, rm, wget, echo)
- [x] Set up an AWS t2.micro instance with 30 GB EBS storage and ssh into this instance
- [x] Install conda on your AWS instance
- [x] Install fastqc in a conda environment named 'week_1' on your AWS instance
- [x] Download some fastq files of RNAseq project (GBA bulk, LRRK2 neurons, etc) using wget
- [x] Install 'filezilla'/WinSCP, or any program capable of 'sftp' and download your fastqc report(s) to your computer
- [x] Evaluate the quality of a fastq file from the report generated by fastqc
- [x] Practice using tab autocompletion on the command line
- [x] Practice using the up and down arrows to cycle through command history
- [ ] Copy your command 'history' to a GitHub document for reference later
- [x] Start using 'screen' to run programs in the background (Ctrl-a, Ctrl-d, Ctrl-k, screen -S name, screen -r name)

### Wednesday: Guide
  1. Find a paper with bulk RNA sequencing. I recommend [this airway paper](https://www.ncbi.nlm.nih.gov/pubmed/24926665), as we may be using this paper's data for more practice later on.
  2. Locate the [EBI](ebi.ac.uk) 'Nucleotide Sequencing' Project page for the paper. [Here is the page for the above paper](https://www.ebi.ac.uk/ena/browser/view/PRJNA229998)
  3. Use 'Select columns' to choose which columns you need. We need the 'fastq ftp' column, and a column that helps us identify which sample is which
  4. Download the 'TSV' (tab-separated values) file and open it in excel.
  5. Use some of the 'fastq ftp' links to 'wget' the fastq files to our AWS instance
  6. Run fastqc on each fastqc file
  7. Install Filezilla, WinSCP or equivalent on your local machine
  8. Add a new 'site': Protocol is SFTP, Host is the 'public DNS' of your AWS instance, Port is 22, User is ubuntu and key file is the '.pem' file you made yesterday.
  9. Connect and download all the 'fastqc' output files
  10. Open the '.html' files in your browser and take a look at the information. Google these quality checks and read the 'Babraham' guidance on them: [Example](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/Help/3%20Analysis%20Modules/4%20Per%20Base%20Sequence%20Content.html)
  
### Thursday: Guide
  1. Access the EC2 instance (ec2-3-11-80-159.eu-west-2.compute.amazonaws.com) (password: trinity)
  2. Install miniconda in your home folder
  3. Install STAR in a conda environment
  4. Download the fastq files from the [airway](https://www.ebi.ac.uk/ena/browser/view/PRJNA229998) project (perhaps divide up the task of downloading)
  5. Download the Gencode primary assembly FASTA and GTF for [human](https://www.gencodegenes.org/human/)
  6. Generate a genome index using STAR: Follow section 2.1 of the [manual](https://github.com/alexdobin/STAR/blob/master/doc/STARmanual.pdf)
  7. Use a for loop to map your fastq reads to the genome index in STAR: See section 3.1 of the manual
```
Example for loop:
for file in *1.fastq.gz ; do echo "STAR --numThreadN 4 --genomeDir folder_where_genome_index_is $file ${file%1.fastq.gz}2.fastq.gz" ; done
```

### Friday: Guide
  1. Our objective is complete mapping the airway fastq files to the human genome reference 38 from GENCODE.
  2. Your AWS instance is accessible using: `ssh -i "msc_tt2020.pem" ubuntu@ec2-18-132-67-54.eu-west-2.compute.amazonaws.com` from the directory in which your `.pem` file is stored.
  3. One person install miniconda, then notify everyone when it is installed.
  4. Each person creates their own environment, including their initials.
  5. Thursday's work is stored in the `/home/ubuntu/thursday` folder
  6. Friday's space is `/home/ubuntu/friday`
  7. To see how much space is free, type `df -h`: You will see that the `thursday` folder is currently almost full.
  8. To see how much space each folder in a given directory takes up, type `du -chd 1`
  9. Using these commands, try to decide whether you can optimise the amount of space you are using in the `thursday` folder (you could do this while waiting for STAR to generate an index in the `friday` folder)
  10. One way to save space is to avoid having duplicates of large files. You could agree upon a single folder to store the fastq files, reference genome files, and STAR index, and then create [symbolic links](https://kb.iu.edu/d/abbe) to your own working folders (or just reference this single shared folder in each of your commands).
  
  ### Monday 11th May: Guide
  - **Today's AWS address: `ec2-18-130-119-110.eu-west-2.compute.amazonaws.com`**
  - [Samtools tutorial](http://quinlanlab.org/tutorials/samtools/samtools.html)
  - [Airway paper, see RNA seq methods section](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4057123/)
  - [Picard, CollectRNASeqMetrics: *Note, picard can be fussy about how the command is written!](http://broadinstitute.github.io/picard/command-line-overview.html#CollectRnaSeqMetrics)
  - [RSeqQC](http://rseqc.sourceforge.net/)
  - [MultiQC: Check out the **modules** section for information on what it needs to compile information from each tool](https://multiqc.info/docs/)
  - [featurecounts](http://bioinf.wehi.edu.au/featureCounts/)
  
  
  1. Sync your personal AWS S3 folder to a personal folder within the `Monday` folder on the instance.
  2. Set up miniconda + an environment with samtools, picard, rseqc and subread.
  3. Convert your SAM files to BAM files, sort them, index them.
  4. Run Picard CollectRNASeqMetrics on each bam file
