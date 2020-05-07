# RNA-seq-analysis
Working on an RNA-seq dataset for pine root tissues colonized by an ectomycorrhizal fungus in a greenhouse drought manipulation experiment (same plant & fungus across different watering regimes)
The goal is to investigate mycorrhizal fungal response to drought through differential gene expression and physiochemical properties 
Genome is now available for this fungus, which was not when Sonya Erlandson was working on this project, and got the samples sequenced. 

cd Volumes/Mykodrive_B3/Andrea


#data:
- RawData: contains raw sequencing fastq files from Sonya
- Tru-Seq3-PE-2.fa: adapter sequences used for trimmomatic

#Results:
- untrimm_fastqc:
  - fastqchtml - untrimmed fastqc results
  - fastqczip - untrimmed fastqc results
- trimmomatic results
  - unpaired_fastq: untrimmed fastq sequences
  - paired_fastq: trimmed fastq sequences, no adapters
- multiqc_data: first round of mutli_qc reports


#masterdf_boxplots.R 
- R file containing the code for the boxplots I've made for phsyiochemical properties of bishop pine




