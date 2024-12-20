# Weekly Updates
Track my progress throughout the course with weekly entries and documents to showcase my work.  

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

*Reflection on the process used last week and how I can make the process work better?* <br>
Last week I mostly ran things interactively which was not the best strategy. Now I am taking advantage of scheduling jobs so I don't accidentally lose progress if my computer turns off. I'm wondering if running with proper resources might fix my incomplete file problem. 

**Week 7 - 10/8/2024**

*What did I do last week?* <br>
Last week I did a lot of troubleshooting - still working on initial processing of bams -> ATCGmap -> vcfs. I played around with scheduling jobs to carry out these computations and it was a lot less intimidating than I thought. The hardest part was getting the timing and memory allocation correct. After a lot of troubleshooting, I realized that my previous strategy was using way to much memory. Basically I was running the program with an allocated 50GB and was using approximately 55GB (I now know how to look up all this information) and so the program was completing but files were just barely getting cut short which made it hard to detect but was causing a variety of issues farther down the line. Lots of learning last week. 

*What do I plan to do this week?* <br>
To overcome the memory issue, I am going back to step 1 and breaking my practice sample down into individual chromosomes. That way it's less work per round so I won't overrun the memory. Everything seems to be going well so far. Mostly just working on writing a "split" program to get all the chromosomes in their own files and then rewriting everything I had previously written to now iterate through all the chromosomes one by one before merging them back together once the heavy stuff is done. So far it's going well. Again just need to calculate the right time and memory for these and hopefully I'll be able to run the full list of samples through this process soon. I've just been doing all this troubleshooting on one file so I'm going to meet with Dr. Watowich this week to chat about how to scale it up to run on the 4000 sample files they have.  

*Are there any impediments in my way* <br>
Same as before, troubleshooting is just a slow process, but I'm learning so much. Also understanding large memory is a new concept for me but very good to learn. 

*Reflection on the process used last week and how I can make the process work better?* <br>
Breaking things up by chromosome is helping with troubleshooting because I can see specifically which files are getting corrupted. I've never really had to consider memory usage before so this has been a good practice in understanding how/why I need to take memory into consideration. 

*Life Long Learning Task* <br>
I took a look around the Career Services website and spent some time reading through their interview tips. I have seen multiple people mention the STAR method but never really looked into it myself. Career services has some good interview tips and links on the STAR method and lots of practice interview questions. I spent some time giving practice answers out loud for some of the questions they listed. I found it's pretty hard to keep it short and sweet (I tend to ramble in interviews) so that's something I will work on moving forward. I think the STAR method gives a good outline of how to narrow down your story and focus on the important points. I've sent out some job apps so I'm hoping to hear back soon and hopefully get to practice some of these interview techniques in real life! 

**Week 8 - 10/16/2024**

*What did I do last week?* <br>
Last week I finalized my first set of scripts. To overcome memory issues, I broke each sample by chromosome and then ran each one through the steps and that has worked well. Once I got that working, I got approval to run the whole batch. Before submitting a "job" you have to specify runtime and memory so I did some experimenting to make sure I set the right amount. That all went relatively well (some jobs timed out and needed to be rerun) and the files started processing. I got all 4000 samples through step 1 (sort) and then immediately maxed out the available space on step 2 (split). 

*What do I plan to do this week?* <br>
To work within storage constraints, I am now going to process in batches of 1000 (I went back and deleted some of what I already output). I'll run all files through the pipeline successfully, then delete unnecessary intermediate files, and then do the next 1000. This should allow me to get through all 4000 without needing the lab to go through the process of buying more storage space. 

*Are there any impediments in my way* <br>
Trying to play tetris with storage space. I also don't want to delete something that I may need later on so I'm trying to look ahead at the next steps but it gets significantly more complicated after this so it's hard to tell. 

*Reflection on the process used last week and how I can make the process work better?* <br>
I think I made good adjustments and I have a good system in place to monitor jobs, submit more jobs, and check for errors. 

**Week 9 - 10/23/2024**

*What did I do last week?* <br>
Last week I continued my battle with memory issues. In my first attempt, I had started to run the scripts (for turning bams into vcfs) but ended up running out of space...again. I did some restrategizing and decided that instead of running all the files one step at a time, I will now run one file at a time through all the steps. This means I can go back and delete the intermediates immediately instead of waiting for 4000 intermediate files to generate then move onto the next step then go back and delete. 

*What do I plan to do this week?* <br>
 This week, I am mostly just waiting for all these files to run. I'm at about 500/4000 so it's probably going to be another week or two. In the meantime, I am looking at next steps. The immediate next step is a list of filtering steps that I think that will be pretty straightforward to figure out once I read some more module documentation. I'm also realizing that I'm getting absorbed in the coding steps that I've been tasked with and I am becoming a little disconnected with the bigger picture. While I wait for these files to run, I am going to focus on reading some more articles and trying to rebuild the context around what I'm doing. 

*Are there any impediments in my way* <br>
Sometimes a file times out and I have to find out which one it was and rerun it. I've been told this is normal and probably something to do with malfunctioning nodes (?). It's not that big of a deal, moreso an inconveinence.

*Relfection on the process used last week and how I can make the process work better?* <br>
The "run each thing through all the steps" instead of "run all the things through one step at a time" is definitely a better approach. 

**Week 10 - 10/31/2024**

*What did I do last week?* <br>
 Last week I was waiting for files to run, so I didn't have much coding work to do. I did test run some scripts for future filtering steps, but I need to wait for everything to finish running before going further. I took some time to go back and read through more detail about what the modules that I'm using are actually doing. Also reread some articles that make a little more sense now that I have a better idea of what is going on. 

*What do I plan to do this week?* <br>
Still waiting for things to run this week. Almost halfway. I'm planning to use my time this week to do more background reading and look into other bioinformatics tools.

*Are there any impediments in my way* <br>
Just waiting. 

*Reflection on the process used last week and how I can make the process work better?* <br>
I appreciated the opportunity to slow down and reabsorb some information.

**Week 11 - 11/6/2024**

*What did I do last week?* <br>
While waiting for things to run, I worked on previewing some of the next steps to get files prepped for QC, mostly working with just one sample file to make sure I have the syntax right. I also did some more reading on general background info like the lab techniques that are done to get this data. There was also a moment when the storage overflowed (not my fault this time haha) and I had to do some damage control - mostly just figure out what got cut off and go back and restart from that point. 

*What do I plan to do this week?* <br>
Still waiting for files to run. We're just about halfway so probably another 2-3 weeks to go if things keep going at this rate. I'm working on running the next merge/filtering steps on a small collection of 5 files that are merged (eventually all 4000 will be merged and go through these same steps). It's slow going but I'm hoping to be prepared for when the full batch of files is ready. 

*Are there any impediments in my way* <br>
Waiting and waiting. 

*Reflection on the process used last week and how I can make the process work better?* <br>
I think I am making good use of my time while waiting and will continue to try to do productive things to prep for the next steps. 


**Week 12 - 11/13/2024**

*What did I do last week?* <br>
Last week I worked more on the preparing the data for QC by looking into the filtering steps and trying them out on some practice data. I'm still waiting for the big batch of VCF files to finish. 

*What do I plan to do this week?* <br>
This week I'm playing around more with the filtering steps and changing up the thresholds of what's considered "quality". Two things we have to consider are keeping high quality samples and sites. With 4000 samples eventually going to be compared, we have to consider that the thresholds might need to be more lenient. For example, if we had 20 samples total we might want to filter to keep samples that cover at least 90% of the total sites observed (by observed I mean ones where we were able to get a confident genotype read) across all samples. But with so many samples there are naturally just more sites so we're thinking about setting the threshold to 75%. I also realized I need to do some little tasks like rehead the files and adjust the order of filtering so I'll work on those things this week.

*Are there any impediments in my way* <br>
Waiting for things to run. 

*Reflection on the process used last week and how I can make the process work better?* <br>I 
think things are going well. 


**Week 13 - 11/21/2024**

*What I did last week:* <br>
Last week I wrote code to rehead my vcf files once they finish running. I also changed the filtering thresholds and read about filtering norms - example: filtering for sample quality before filtering for site quality. Finally, I checked in on the large batch of files that have been running for weeks to rerun any that timed out. 

*What I plan to do this week:* <br>
This week I'm starting to think about timing and scaling my filtering steps to work on the 4000 merged files when they're ready. I'm currently testing it out on 5 merged files and trying out different approaches to see what goes the fastest. I've been reading a lot about a new (new to me) tool called plink. There's some weirdness with file formats and converting back and forth so I'm working on how to sort all that out but plink definitely seems to filter faster than my previous approach.

*Impediment(s) in my way:* <br>
Long run times make trial and error take forever.

*Reflections on the process I used last week:* <br>
I think it's good to switch it up and try out different methods and learn about new tools. 

**Week 14 - 12/4/2024**

*What I did last week:* <br>
Last week I continued to monitor my big batch of files, rerunning when they timed out or cancelled. I also played around with filtering steps on my sample set looking at Hardy Weinberg Equilibruim and Linkage Disequilibrium filters. Turns out my sample set is too small for these to acccurately work so I'm just going to wait until the big batch is done. I have a good idea conceptually of what needs to happen so I think this is fine. 

*What I plan to do this week:* <br>
The big batch of vcf files finished yesterday!!! Very excited. So this week I'm working on double checking that everything went as planned. Then it's time to index, merge, and reheader everything. I've already practiced these steps on a small sample so I just need to scale it up for the large batch now. 

*Impediment(s) in my way:* <br>
Everything is going well. 

*Reflections on the process I used last week:* <br>
I think choosing to stop playing around with the same set was a good idea. I learned as much as I could about the next steps but now it's going to be up to seeing how the large merged file reacts to all the filtering steps and adjust accordingly.

**Week 15 - 12/9/2024**

*What I did last week:* <br>
Last week I started the quality control portion of my project. With the files finished running, I need to merge them into one big file and then reheader them all to reflect the sample they belong to. To do that, they need to first be indexed. So last week I indexed and then started merging. After a few days of running, it turns out I did not give the merge nearly enough memory or time so that ended up failing.

*What I plan to do this week:* <br>
In the first merge attempt I gave the job 200G of memory and 76 hours to run and it timed out and the resulting file was way too small. I have done some invesigating and I think the bcftools merge command requires all files to be open at once in memory (~ 3.5T) so I am trying to find a more efficient way to do this. I found a forum post that suggests doing it in smaller batches and then merging the batches so I will be working on that this week. As a backup, I could just schedule a super high memory and time job but that would probably take forever to be scheduled and also I still have no concept of how much time it would take. It would be unfortunate to wait a week for it to schedule, wait 2 weeks for it to run, only for it to fail again. 

*Impediment(s) in my way:* <br>
Understanding how to work with big files is an ongoing struggle.

*Reflections on the process I used last week:* <br>
I made a good attempt last week and this week I have a better idea. 


