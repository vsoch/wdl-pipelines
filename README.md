# Pipeline Reviews

Here I am going to do the following:

 1. Review ENCODE pipelines and comment on the documentation.
 2. Attempt to run the pipeline with DNA Nexus and Google Cloud
 3. Also give a try at a biological interpretation of the result

Since I don't want to do this twice, I'm going to write the documentation as I go, and render
into a web interface. You can see the documentation at [https://vsoch.github.io/wdl-pipelines](https://vsoch.github.io/wdl-pipelines) and my initial notes and suggestions (deprecated) below.

 - [Chip-Seq](#chip-seq-review)

## Chip-Seq Review

### Pre-Review

 1. The pipeline that I found is [here](https://www.encodeproject.org/chip-seq/histone/) and I'm not sure if this is the correct one, because there is another one with the only difference that it's for transcriptome. After seeing links to "instances" on this page, I figured out the pipeline "alien code" has it's own page at [this url](https://www.encodeproject.org/experiments/ENCSR970FPM/), but I'm not sure where to go from here (this appears to be a summary of an experiment).
 2. From the main page I started at, I was able to follow the link to create an account on DNANexus (not knowing what it is). I am not sure if I need to pay for this on my own (I hope not!). It might make sense for some tutorial to mention what it is, for noobs like me. I'm guessing it's an online platform to run genomics pipelines? Are there group or institution associations?
 3. I'm reading the same page, and again seeing there are links to "pipeline instances" (the pages with the pipeline identifiers that have tags as "experiment summary.") I'm not sure what an instance refers to, but I like the tag for "Encode Stage 3" because that tells me that (I think) it's something I should be interested in. I typed in [this link](https://www.encodeproject.org/experiments/ENCSR970FPM/) to match with the code I got to try, and I didn't know where to go from there. This appears to be describing (someone else's experimental data). I went back to the original page.
 4. Okay, now I'm a bit confused - the first set of links appear to be for different kinds of experiments (that were replicated) and then farther down a description of the pipeline inputs/outputs (this makes sense to have here) and below that a more hidden section with "References" that seem to be publications.
 5. Where are the "Hey Friend, let's get started!" sections?

### Suggestions

 - Many people will stumble on a page exactly like this from a search. I'd really like to have steps, found or linked right here, that walk me through how to run this pipeline. It should be in the line of a friendly getting started tutorial, intended for someone like me that hasn't a clue what's going on. Right now I'd just be guessing that I need to dig through a Github repo, or some older publication, or DNANexus (and I don't know what it is) to get started. Coming from someone who has never used this site, it's not clear to me how to get started.
 - If the overview "last updated" date is manually done, it might make sense to have an automated date that updates when the docs are last built.
 - I've never used these pipelines so I'm not familiar with the coding schema (e.g., ENCSR970FPM). It might make sense to briefly mention this "the alphanumeric string is a unique identifier for..."

I think I'll accomplish more just writing the documentation I'd expect on my own.
