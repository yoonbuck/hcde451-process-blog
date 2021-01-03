---
layout: process.njk
title: voice interaction
stepNo: 5
active: true
date: 2020-11-09
artifacts:
  - ["all dialogs", "dialogs"]
  - ["flowcharts", "https://cdn.yoonbuck.com/hcde451-www/5-voice-interaction/flowchart.pdf"]
---

# design

This week's goal of prototyping voice interactions sent me searching for a new project idea—while the whirlibird is fun, I don't think adding voice assistant functionality is the killer feature it's been missing this time. So I hope you will forgive this interruption to your regularly scheduled adorable dog content!

I stumbled upon my idea for this week while working in a research group led by <a href="https://www.hcde.washington.edu/atman" target="_blank">Dr. Cindy Atman</a>. Building off of her ongoing research on the concept of <a href="https://www.youtube.com/watch?v=pV3qEAIeiSY" target="_blank">design awareness</a>, we're creating an app to help people track their design process in realtime.

For this week's project, I explored how this app's functionality might be implemented as a digital assistant, which I affectionately named Dizzy. This assistant has the ability to start and stop tracking a user's design process while they work on various projects. While tracking, the user can let Dizzy know what design activities they're engaging in, in order to help Dizzy build a record of their process. Afterwards, the user can query Dizzy for various information about their design process.

The purpose of this investigation is to evaluate the viability of this functionality as a voice assistant as opposed to the more conventional mobile app format that's we're currently developing.

# prototype

I began by identifying five key tasks that the virtual assistant would need to be able to perform. I came up with the following five tasks:

- **Start project tracking:** begin a tracking session for a particular project
- **Change activity status:** toggle specific activites on or off
- **Stop tracking:** end a tracking session
- **Manage projects:** create new projects or get the most recent project
- **Query activity data:** ask questions about the tracking data from a project

After thinking about the information and context that would be necessary for the user to provide as well as the information that the virtual assistant should include in its response, I began to write sample dialogs for each of these tasks. One example dialog, for the key task "start project tracking," looks like this:

<div class="page--bq-dialogs">

> **Dizzy, start tracking.**
> *Sure. What project are you working on?*
> **I'm working on my portfolio.**
> *Okay! I've started tracking for portfolio.*

</div>

To help me refine these dialogs, I tested these out with two of my classmates playing the roles of user and assistant. I found this step to be a really fascinating aspect of designing for voice interaction, as I was drawn to the idea of a prototype evaluation process which doesn't use any technology at all! It also turned out to be super useful, as I was able to identify phrasing that seemed awkward for the speakers or to a listener and adjust the language used for the queries as well as the assistant's responses to feel more natural.

In total, I created <a href="dialogs" target="_blank">20 dialogs showing different combinations of user requests and possible errors</a> across the five key tasks. I also created <a href="https://cdn.yoonbuck.com/hcde451-www/5-voice-interaction/flowchart.pdf" target="_blank">flowcharts to show the possible branching flow of conversations and additional error states.</a>

# analysis


Ultimately, it's difficult to know how effective my voice assistant could be with only the limited testing I was able to do with my early dialogs. Still, I'm very optimistic about the results. It went quite smoothly and the people who I tested with said that the use case seemed very reasonable and the dialogs were straightforward. I think there's still improvements that could be made, particularly with the responses relating to queries and the information provided upon ending a task. I would need to do more research to find out what the most useful information to provide would be.

To be honest, I was somewhat hesitant going into this process. I've always been a bit weary of voice interfaces and particularly voice assistants. Personally, I don't find the concept particularly compelling and I don't know a lot of people who use voice assistants for more than fairly basic tasks or as a novelty. Still, it seems like this is definitely a rapidly growing technology, so it was a great opportunity for me to get out of my comfort zone and learn a little bit more about designing for voice.