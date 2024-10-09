# Weekly Updates
Track my progress throughout the course with weekly entries and documents to showcase my work.  

## Weekly Entries 
**Week 1 - 8/30/2024**

My goal for this week was to orient myself with the course expectations and to start defining my goals for the semester. I watched the intro video and posted an intro comment on Piazza. I also had a meeting with career services to think about getting ready for the job search. The advisor also pointed me to some useful resources like O.net and the CU alumni contact page. I did some career exploration via O.net and I'd like to set up some informational interviews with alumni to learn more about potential career paths. I am currently waiting for my account to be authorized. Hopefully that happens soon and next week I can reach out to some folks on the network and set up a few interviews. In the meantime, I looked into some job descriptions for positions I am interested in - mostly entry level data science or data analyst roles. I wrote down a list of some technical requirements that I am unfamiliar with so I will need to look more into those. These could be a good starting point for a larger semester project. Currently my goals for next week are 1) to set up a "master resume" with extensive detail so that I can pull sections from it as I apply to different jobs in the coming months and 2) identify coding project ideas. 


**Week 2 - 9/5/2024**

*What did you do last week?* <br>
  Last week I had a meeting with career services about some job searching basics. I did some research looking to job postings to get an idea of requirements for different positions. I'm mainly looking into data analytics roles (or maybe a junior ML role if that exists) in industries that overlap with natural sciences or sustainability. I used this info to start putting together some skills that I would like to develop. Some things currently on my list - Power BI, Tensorflow, and SQL. I also have been thinking about whether or not I'd like to go to grad school someday so I used some time this week to look into different areas of research. In my job exploration I ended up finding a part time job to apply to (low hopes but good to practice putting together the submission materials) I also did some reading about github websites and set mine up in a very basic format. Still needs some work. 
 
*What do you plan to do this week?* <br>
  Currently I am working on defining my goals for this class - trying to decide if I want to go all in on a challenging project or work on small projects to develop specific skills or certs. I've been searching github to get an idea of what a start to finish independent project even looks like. Leaning towards a bigger project just because I haven't done anything like that before. Since I know I want to work with data, my goal is to find a dataset that looks interesting and start to develop project ideas from there. I am also planning to reach out to a contact that works in an evolutionary bio lab to set up an informational interview and learn more about the field (and maybe be able to volunteer?) 

*Are there any impediments in your way?* <br>
  At the moment my only impediments are self-imposed. I'm feeling slightly overwhelmed by all the information out there and how much I do not know. I am finding it hard to focus in on something.

*Reflection on the process you used last week, how can you make the process work better?* <br>
  Last week was very much a hodge-podge of me reading lots of information and going off on tangents. I think completing the official project proposal and adding in week by week details will help me focus future weeks to be more productive. 

**Week 3 - 9/11/2024**

*What did you do last week?* <br>
  Last week I did a lot of research into potential project ideas. This led me to reach out to a contact at an evolutionary genetics lab and set up a volunteer opportunity with them. 

*What do you plan to do this week?* <br>
  -This week I met with my lab contact to get an idea of how to start prepping to work on the project. My plan for the rest of week will be spent learning R basics, reading some research papers, and watching youtube videos on epigenetics and DNA methylation data pipelines. <br>
  -Write and submit proposal <br>
  -Try to get a theme on my website (troubleshooting why there is no theme button like the tutorial says there should be) <br>

*Are there any impediments in your way?* <br>
  -Currently waiting to get added to a server so I can start looking at the data I'm going to be working with <br>
  -Feeling a little underprepared just jumping into a bioinformatics project with no prior experience 

*Reflection on the process you used last week: How can you improve it?* <br>
  Last week I was still in the indecisive phase so I am glad that this week I have a steady plan started. It feels good to start taking tangible action. Going forward, I think setting realistic weekly goals is going to be key. 

**Week 4 - 9/19/2024**

*What did I do last week?* <br>
  Last week, I met with Dr. Watowich to get generally acquainted with what I'll be working on. I then did a lot of research and reading about topics related to my project - DNA methylation, R, processing sequence reads, and generally just refreshing my memory on some genetics concepts. 

*What do I plan to do this week?* <br>
  This week I am working on setting up my access to the computer cluster that the lab uses. I have a meeting with Dr. Watowich to get acquianted with the cluster and talk about first steps. 

*Are there any impediments in my way?* <br>
  Little bit of information overload - new computing environment, working with R and Bash, and getting up to speed with the project. 

*Reflection on the process used last week, and how can I make the process work better?* <br>
  I think last week I tried to cram a lot of new information at once. Going forwards, I will break up my time across multiple days so that I have a chance to process information and understand it better. 

**Week 5 - 9/26/2024**

*What did I do last week?* <br>
   Last week I got connected to the group computer cluster and watched all the training videos on how the cluster works, using Bash, and scheduling jobs. The rest of my time I spent getting used to Bash, setting up my directories, and started looking at the first steps of processing the data. I am starting from BAM files (so the raw sequencing reads have already gone through some quality control and alignment). 

*What do I plan to do this week?* <br>
  This week I am working on taking those BAM files and sorting them, then converting into a .vcf file to extract genotypes. This is all done with premade modules (samtools, cgmaptools) so I am mostly reading documentation trying to figure out how to install/load these modules and what arguments they need. 

*Are there any impediments in my way?* <br>
  I have an example script to follow so that has been my guideline while doing all this. The hardest part has been reading through the documentation to figure out what arguments to use. It also takes like 20-30 minutes to run one command on one file so it's slow going. But eventually when I get the scripts figured out I will send a big batch to the scheduler and I won't have to sit there and wait.  

*Reflection on the process used last week and how can I make the process work better?* <br>
  Last week was still a lot of logistics just orienting myself to the project and the cluster. This week I have started writing code so I'm excited to see how that goes and come up with some strategies going forward. 

**Week 6 - 10/3/2024**

*What did I do last week?* <br>
Last week I worked more on processing the bam files into a vcf format. The steps I am working on is: 1) sorting bam file, converting bam file to atcg, extracting SNPs from atcg, then filtering for good quality reads. This is all done with modules so it's a couple file paths and then about 10 lines of code, so not that much but it's taking forever to get it working. Last week I got a file to run all the way through and that was exciting until I realized my final file only included 2 chromosomes. 

*What do I plan to do this week?* <br>
This week I am working on troubleshooting why my final file only has 2 out of 23 chromosomes. I'm trying a couple different troubleshooting methods but it's really slow going since everything takes so long to run. While I wait for things to run, I am working on read ahead in the example scripts and getting ready for next steps. 

*Are there any impediments in my way* <br>
Troubleshooting takes forever. Running one file takes like 15 hours and if something goes wrong I make a change and then wait another 15 hours. Very slow going. 

*Relfection on the process used last week and how I can make the process work better?* <br>
Last week I mostly ran things interactively which was not the best strategy. Now I am taking advantage of scheduling jobs so I don't accidentally lose progress if my computer turns off. I'm wondering if running with proper resources might fix my incomplete file problem. 



