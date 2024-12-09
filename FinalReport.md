# Final Project 

Nicole Cosmany <br>
CSPB 3112 Professional Development

**Project**: DNA Methylation Project 

**Introduction**: 
My goal for this project was to explore my interest in computational biology. I wanted to apply my programming skills to real world biological data and also confirm whether or not I wanted to pursue graduate school next. I reached out to an acquaintance in the Lea Lab at Vanderbilt and was able to get connected as a remote volunteer working on one of their ongoing projects. Through this project, I learned a variety of skills including running jobs on a computer cluster, exploring applications of computational biology, and processing DNA methylation data.

**Background**: 
This project was a really great opportunity not only to practice my programming skills but to learn about applying data analysis techniques to largescale biological data. The specific project I worked on was 1) building a pipeline to process DNA sequencing reads from a BAM format to a VCF format and 2) performing quality control. 
The starting dataset was a group of 4204 BAM files, each containing DNA methylation data for individuals from 3 distinct populations. The raw data is a binary file consisting of fragments of genetic reads and the steps of the pipeline sort them into their corresponding chromosomes and extract genotype at each site. Genotype needs to be “extracted” because multiple reads must be aligned to cover a certain site and then it’s a question of probability to make a definitive call. We also match with a reference human genome when making these calls. Plus, since this is methylation data, the C’s that show up as C’s are unmethylated and the T’s could be either unmethylated C’s or true Ts. The modules that I used are able to take all these this into account and statistically predict genotype and include a certainty score, which we can then use to make decisions about what data to keep. At the end of this genotyping stage, we have a VCF file.

After generating the VCF files, the next step I worked on was quality control. The goal here was to ensure that all samples are correctly labelled at the individual and population level. This stage included merging all the files together into one big file and then passing the data through a series of filters to remove individuals with too much missing data, sites with too much missing data, low quality reads, and confusing C/T sites. Then we are left with a cleaned dataset that we can evaluate using PCA and a relatedness matrix. I am currently in the middle of this step.

**Methodology, Materials and Methods**: 
I was lucky to have a good support network throughout this project. First, I had an excellent mentor, Dr. Watowich, who is a postdoctoral researcher in the Lea Lab and my direct contact. We set up weekly check-in meetings where I was able to share my progress, troubleshoot issues, and ask career questions. In the early stages of the project, I was given some example scripts from Dr. Watowich’s colleague who had made a similar pipeline. This was a helpful starting point so I knew what kinds of modules to use and the general steps. As the project progressed, we had to go “off script” and conduct some filters unique to our dataset. Dr. Watowich provided general guidelines about what needed to happen (for example: remove low quality reads, remove individuals missing too much data, etc.) and I would read online about different ways to do this, run the idea by her, and then proceed. 
Since my code mostly consisted of piecing together premade bioinformatics modules, I read through a lot of documentation. This was helpful for understanding not only what flags to pass to the module but also different ways to increase efficiency.

**Results**: 
The first big skill I learned in this project was how to use a computer cluster. This included simple things like downloading and loading modules, basic navigation in bash, running files interactively, and running files through SLURM (the cluster job scheduler). The datasets I was working with were huge so I had to schedule most jobs to be sent to a node on the cluster. I had to do quite a bit of troubleshooting trying to figure out how much time and memory to allocate and how to determine if a job ran successfully. I also learned to optimize my tasks – for example instead of running something as a loop in a single file, I could split it up into individual jobs and run them all at once. I also ran into a situation where I generated way too many large intermediate files and overflowed the storage, so I learned to strategically manage intermediate files. This was a great learning experience since I would like to continue working with large datasets and now I have learned some strategies for working with big files.  
The next broad skill I learned was the general flow of processing DNA methylation data – from BAM to VCF to filtering and so on. All the steps were carried out in bash so I learned how to call other modules and pass the appropriate flags. I read through a lot of documentation and by the end I definitely felt like I improved in how to read and use documentation. I also felt like I have a relative sense of the utility of common modules and different thresholds used for various filtering tasks.
Notably, I also learned a lot of conceptual information about DNA methylation, molecular biology, and genomics. I read through quite a few papers at the start of the project to get acquainted with the lab’s work. This was really helpful in aiding my decision to apply to graduate school and what kinds of programs to apply to.
In regards to my specific measurable results – I implemented a BAM to VCF pipeline and generated 4204 VCF files. I also accomplished about half the quality control measures and will continue working on these. I did not get to the IMAGE statistical analysis to extract MeQTL sites, which was my original end goal. 

**Discussion / Reflection**:
My initial goal was to apply the IMAGE statistical package in R in order to extract MeQTL sites. The BAM to VCF pipeline took much longer than I initially expected. (After finishing the script, it took the files about 2 months to run). At the mid semester check-in I changed my goals to include finishing the pipeline and performing quality control. Again, due to waiting for files to run, I am about halfway through the quality control.
Overall, I feel very happy with my project results. I learned so much about managing a general workflow in addition to specific computational biology skills. Even while waiting for long runtimes, I feel like I still made good use of my time – practicing future steps, reading documentation, and constantly monitoring the running jobs for errors. Having weekly meetings with Dr. Watowich was also a huge bonus and I am so lucky to have that kind of mentorship to make this project successful.

**Conclusion**: 
I have really enjoyed this work and will continue to volunteer with this lab and project after this semester. I will definitely complete the quality control stage, which will be a neat way to link to some fun topics I’ve learned in other courses (PCA and a relatedness matrix). And this will incorporate some R visualization so I will get to practice a new language. My goal is to keep working about 5 hours a week with this project and hopefully get to the IMAGE analysis stage in the next few months.
My goal this semester was to figure out my next steps after completing this program in 2025. With my original Bachelor's degree in Biology, I thought I wanted to pursue computational biology, and this project confirmed that it's the right path for me. I really value hands-on experience and this was the perfect opportunity to explore my interests and learn that I really love genomics. It’s such a neat way to combine all the things I am interested in: programming, data science, and biology. This inspired me to apply for graduate school with the goal of starting a PhD program next fall. If all goes well, I'm excited to continue to explore genomics research as a graduate student and in my future career.

**References**:

Documentation: <br>
[Cgmaptools](https://cgmaptools.github.io/cgmaptools_documentation/what-is-cgmaptools.html) <br>
[Plink](https://www.cog-genomics.org/plink/) <br>
[Bcftools](https://samtools.github.io/bcftools/bcftools.html) <br>

Github with example scripts : [here](https://github.com/Cec701/genetic_architecture_DNAm_rhesus/blob/main/RRBS_processing/trim_map.sh)

Papers: <br>
https://www.nature.com/articles/npp2012112 <br>
https://www.google.com/url?q=https://www.biorxiv.org/content/10.1101/2024.09.09.612068v1.full.pdf&source=gmail&ust=1733518670402000&usg=AOvVaw13KWoXoATux556mxw_yN5Y <br>
 + an unpublished paper by Christina (PhD student whose github is linked above) <br>

My github repo with finalized scripts from completed steps: <br>
[here](https://github.com/ncosmany/DNA_methylation_proj.git)

