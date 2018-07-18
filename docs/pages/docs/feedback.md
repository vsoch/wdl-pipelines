---
title: Feedback
sidebar: main_sidebar
permalink: feedback
folder: docs
---

Here is some general feedback for using the pipelines.

## Dependencies

It's really hard setting up new software, and the effort should be minimized for
the user as much as possible, especially given that multiple software languages and
platforms are used. I would recommend:

### Software
 - providing software in containers - modular is best. For example, cromwell should be used via a Docker container, and the same with DNAnexus and the various associated tools. I'd say the one exception might be gcloud because it's already available on instances. This is important because there is a threshold that a user reaches when they subconsciously think "this is too hard" and probably stop the tutorial and give up. We don't want them to reach that threshold.

### Data

 - the hardest part about doing these tutorials was the data. I didn't know **what** the files were, there were a ton of them, I didn't know **where** they were, and I was expected to edit input files to make it work with a platform of choice. This should be done as follows:
   - an example input data, along with it's corresponding file, should be offered **ready to go** for each example.
   - for each input file, a verbose description of what the data is (with links if necessary for further explanation) should be provided. The docs must be written for the least experienced user, and you can assume that the least experienced user knows nothing.

## Ordering of Solutions

 - streamline the primary documentation to describe the easiest solution, and provide links to others. For example, if I'm reading a page for the first time and there are 3 ways to do something, although this might be great because I have choice, as a new user I'm a bit overwhelmed because it's very possible (likely) I don't really know. Instead of putting ALL the content on one page, limit the content to just the primary instructions, and add **links** to additional information.
 - The exception is the higher level (e.g., using Google Cloud vs. DNAnexus) because this I would have a preference for. Along with the previous point, we should consider that the user might not have preference for the platform (e.g., they will invest by chance / suggestion) and in this case the order of platforms should be shown in the order of **our** preference. If we think Google Cloud works the best, or is more cost effective, etc., it should come first.

## Tone

 - Don't forget that the person reading it isn't a robot. The tutorials shouldn't come across as immature, but they don't need to come across as academic papers either. It's okay to write as if you are talking to a person, and throw in the occasional joke! And if there is a robot reading it? I'm sure he will appreciate it too.

## Resources

 - Pages should generally start and/or finish with a "Resources" set of links that provides easy access to resources mentioned in the tutorial, or other resources for learning that might be helpful. The user is likely to come back to the page at a future date looking for something, and this makes it easy to find some external link without needing to re-read content.
 - It's confusing if an input file is mentioned (e.g., input.json) that doesn't exist anywhere.
 - Always start the user at the base of a folder (e.g., a repo clone) and guide them perfectly from there. If something is in a subfolder, don't assume they will find it.

I tried to put together the example walk through in this repository to be (somewhat) closer to what I describe above, although there is still ample work to do, of course! I hope that this is helpful.
