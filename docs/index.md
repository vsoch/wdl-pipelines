---
title: WDL Pipelines
keywords: encode,containers
sidebar: main_sidebar
permalink: index.html
toc: false
---

This documentation will help you to get started running the Encode WDL Pipelines. Continue reading based on what best describes your need:

 - [Pipelines](#getting-started): Getting started to run a pipeline.
 - [Developer](#development): you want to develop an existing or create a new pipeline.

This is a supplementary work in progress for the official documentation that is hosted at the main [wdl-pipelines](https://encode-dcc.github.io/wdl-pipelines/) page.

## Getting Started
You will first set up required dependencies, and then proceed with the pipeline of your choice.

 - [Setup](/setup) all of the pipelines require Cromwell and Docker. Let's set this up first.

After setup (which is brief for now) you can proceed by selecting a particular pipeline you want to run. Within these documentation bases are included instructions for running locally and with several cloud services. All options use Docker and Cromwell as a controller, so you should have already the minimum dependencies. Let's go!

 - [Chip-Seq](/pipeline-chip-seq) The ChipSeq pipeline

## Development
If you are a developer and want to contribute to a repository, you will need to clone it and set up your workspace accordingly.

 - [1. Prepare your Workspace](/github): The first step is to clone a repository to your Github account, and download some sample data.
 - [2. Github Development](/development): if you aren't familiar with the Github flow to checkout branches for new features and changes.
 - **3. Get help** If you need help, please don't hesitate to [reach out]({{ site.github.url }}/issues) and we will help you!


<hr style="margin-top:20px">

<div class="row">
  {% assign loopcount = 1 %}
  {% for post in site.posts %}

   {% if loopcount < 4 %}

   <!-- Parse news-->
   {% if post.category == "news" %}
   {% assign loopcount = loopcount | plus: 1 %}
   <div class="col-md-4">
      <h2><a class="post-link" href="{{ post.url | remove: "/" }}">{{ post.title }}</a></h2>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <p>{{ post.content | truncatewords: 20 | strip_html }}</p>  
   </div>
   {% endif %}

   {% if post.category == "releases" %}
   {% assign loopcount = loopcount | plus: 1 %}
   <div class="col-md-4">
      <h2><a class="post-link" href="{{ post.url | remove: "/" }}">{{ post.title }}</a></h2>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <p>{{ post.content | truncatewords: 20 | strip_html }}</p>  
   </div>
   {% endif %}
   {% endif %}

  {% endfor %}
</div>
