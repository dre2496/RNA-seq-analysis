# RNA-seq-analysis
Working on an RNA-seq dataset for pine root tissues colonized by an ectomycorrhizal fungus in a greenhouse drought manipulation experiment (same plant & fungus across different watering regimes). 
The goal is to investigate mycorrhizal fungal response to drought through differential gene expression and physiochemical properties. 
The genome is now available for this fungus(Suillus pungens), which was not when Sonya Erlandson was working on this project, and collected and sequenced samples.

cd Volumes/Mykodrive_B3/Andrea


/data:
/RawData - contains raw sequencing fastq files from Sonya
/masterdataframe.csv - contains bishop pine physiochemical properties under chronic and acute stress conditions measured by Sonya
/Tru-Seq3-PE-2.fa - adapter sequences used for trimmomatic
/hs_err- error messages from trimmomatic that were redone manually/individually 


/Results:
/untrimm_fastqc:
  /fastqchtml - untrimmed fastqc results
  /fastqczip - untrimmed fastqc results
/unpaired_fastq - untrimmed fastq sequences
/paired_fastq - trimmed fastq sequences, no adapters
/multiqc_data - mutli_qc reports for trimmed sequences 
/kallisto_analysis - files needed for running kallisto 
    /chronic.stress.roots - results from pseudoalignment of transcriptome provided by JGI Filtered Models ("best")
    /Suipun1_GeneCatalog_Transcripts - JGI transcriptome FASTA file used to build kallisto index 
    /Suipun1_GeneCatalog_Transcripts_index ^
    /suipun.metadata.csv - metadata used for sleuth analysis
    
/Rscripts: 
  /masterdf_boxplots.R - file containing the code for the boxplots I've made for phsyiochemical properties of bishop pine
  /statisticalAnalysis.R - files containing ANOVA and Tukey HSD tests for physiochemical data (masterdataframe.csv) 
  /suipun.metadata.csv - duplicate of file needed for sleuth analysis
  /kallisto_analysis.R - post kallisto analysis, sleuth 
 
  
/SuipunStandDraft_copy - file containing JGI Suillus Pungens Genome and Transcriptome from JGI 
