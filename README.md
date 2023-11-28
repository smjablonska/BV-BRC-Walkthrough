# BV-BRC-Walkthrough
Hi! This is the BV-BRC Walkthrough for various data 

There are two single read files included in the file section

SRA accession numbers are also good practice: SRR390728_1.fastq.gz // SRR390728_2.fastq.gz

# Why is BV-BRC helpful? 

Ability to utilize multiple software's at the same time: 
Genome assembly

Combines the data, technology, and extensive user communities from two long-running centers: PATRIC, the bacterial system, and IRD/ViPR, the viral systems.

Open-source tools for data analysis and genomic annotation

## What functions are possible in BV-BRC? 

Upon going into the "Tools & Services" section - there are a multitude of tools that are futher categorized based on user needs. Such needs as Genomics, Phylogenomics, Protein tools, Metagenomics, Transcriptomics, and Utilities.

This repo specifically focuses on Genome Assembly, Genome Annotation and Metagenomic Binning. 

<img width="438" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/bca94980-016c-4612-a7ff-be54a4d2dddf">

## Uploading your data 
To upload your data, navigate to the button on the lower right hand side labeled "Upload". 

Once clicked, there will be a chance to select files on computer or drag and drop them. 

There is also an upload button on the left hand top of the page. Once option menu is clicked, there are a multitude of classifications for your data such as contigs, reads, aligned DNA fasta, etc. 

All files upon successful downloading will be present in home folder. There is also a percentage that is continuously updated once each file is successfuly uploaded. 

<img width="536" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/71fee0ba-6c00-49e0-8d95-7027118587c4">


When submitting any job, the job section (button right of upload) will populate in a number depending on which stage of the processing the request is in. 

Queue in grey, running in yellow, and done in green. 

In image below, the left hand is shaded in green, denoting successful run of job. Following columns show ID of job, job required, output name, date of job submission, date of job start and date of job end.

<img width="653" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/9a3dc8a2-30dd-42b1-8dc9-c3ad66cfb874">

**If something goes wrong, such as the job failing to run - the left hand writing will say "failed" in the color red. 

## Genome assembly
To start off your genome journey - you will upload either a paired read library (left and right sequencing pairs), a single read library, or a SRA run accession. A library NEEDS to be moved into the "Selected libraries" portion on the right hand side or the job will not run!!
Always remember to note an output folder and output name of job.

<img width="353" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/bba320d0-52cd-44d6-be1e-21b95e165def">

There are multiple parameters for assembly strategy: 
*I suggest auto because genome assembly will optimize the job depending on the tools.

<img width="148" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/97deab6b-c575-4944-82be-b639c4f24ee9">

Once job is complete, there is an array of results you can access. One of importance is the Name_of_output_file_AssemblyReport.html

<img width="381" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/ef43af51-2fa9-45da-b141-27a9916b4299">

Results: Name_of_output_file_AssemblyReport.html

The bandage plot is a tool for visualizing assembly graphs with connections. For people who have taken/know about bioinformatic theory - a de Brujin Graph. 

<img width="331" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/1d66e5f2-9e83-4dcc-8a6d-945c131aa998">

In the assembly process section, the tool, tool version and command line commmands are seen. Such details provide transparency in the process conducted to assemble genome. 

<img width="387" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/eec79f81-e487-42ff-a00a-02a96c300371">

## Metagenomic binning
Metagenomic binning is the process of grouping reads or contigs and assigning them to individual genome. 

Input for metagenomic binning consists of either putting in two left anf right reads, one single read or inputting an SRA accession ID. 

AGAIN - whichever library is being used needs to move into the selected libraries portion by clicking the arrow pointing to the left of each respective library. 

For parameters, always choose an output folder and output name. Parameters for assembly strategy and organism of interest is up to you.  

<img width="329" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/74b25b5c-b637-482d-98e4-86c230042dd4">

Once job is complete, there is an array of results you can access. One of importance is the BinningReport.html 

<img width="367" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/650ec3f1-e809-4fc2-aaf7-c878b9a2d639">

Results: BinningReport.html 

Metagenomic binning gives useful overview information to assess your genome such as completeness, contamination, coarse consistency, etc. 

<img width="533" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/1100cbea-0397-428e-8a3d-34e8fde5e193">


## Genome Annotation
For genome annotation, the use of a single contig is needs. You can use the single read generated from the genome assembly service. 

You can annotate your recipe and make it more specific with parameters of taxonomy name and ID. 

Always remember to label your job and select an output folder. 

<img width="383" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/8de07b74-fa8f-4bbb-915e-b43dac258cdd">

There are multiple parameters for annotation recipe: 

<img width="163" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/58debc7e-f48a-40dc-997b-e48197d3d5af">

Once job is complete, there is an array of results you can access. One of importance is the GenomeReport.html 

<img width="624" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/91bee03a-6668-46fc-9f34-e7dc22dac0a3">

Results: GenomeReport.html 

Results in this section give insight into evaluation group, DNA size, contigs,and potential/predicted roles in genome. 

<img width="402" alt="image" src="https://github.com/smjablonska/BV-BRC-Walkthrough/assets/103958073/f0facdba-55ea-440c-8d6f-8ffe0f909bd9">

## Acknowledgments
Credits to the original website!

* [BV-BRC][https://www.bv-brc.org]

