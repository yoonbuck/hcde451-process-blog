---
layout: standalone.njk
title: voice interaction dialogs
date: 2020-11-09
---
<div class="page--bq-dialogs">

Jump to dialog samples for a key task:

1. [Start project tracking](#key-task-1)
2. [Change activity status](#key-task-2)
3. [Stop tracking](#key-task-3)
4. [Manage projects](#key-task-4)
5. [Query activity data](#key-task-5)

<a id="key-task-1"></a>

# start project tracking

## no context

> **Dizzy, start tracking.**
> *Sure. What project are you working on?*
> **I'm working on my capstone project.**
> *Okay! I've started tracking for capstone.*

## project in request

> **Dizzy, start tracking capstone project.**
> *Okay! I've started tracking for capstone.*

## existing tracking session

In this scenario, the assistant encounters the error where a project is already being tracked. It needs to effectively communicate its constraints to the user, and make the options for how to proceed clear.

> **Dizzy, start tracking portfolio.**
> *You're currently tracking capstone. Since I can only track one project at a time, do you want me to stop tracking capstone so I can track portfolio?*
> **Yes.**
> *Okay. I ended your tracking session for capstone and started started tracking for portfolio.*

## new project

In this scenario, the assistant encounters the error where a user requests a project that doesn't exist. It helps the user create this project, if desired.

> **Dizzy, start tracking.**
> *Sure. What project are you working on?*
> **I'm working on my portfolio.**
> *I can't find any existing project with that name. Do you want me to create a new project called portfolio?*
> **Yes, please!**
> *Okay, I created the project portfolio and started tracking.*

<a id="key-task-2"></a>[back to top](#)

# change activity status

## start activity

> **Dizzy, I'm modeling.**
> *Okay, modeling is active.*

## start with current activity

> **Dizzy, I'm gathering information.**
> *Are you still modeling?*
> **Nope, I'm done modeling.**
> *Okay. Gathering information is active and modeling is inactive.*

> **Dizzy, I'm gathering information.**
> *Are you still modeling?*
> **Yes.**
> *Okay, now gathering information and modeling are both active.*

## switch activity

> **Dizzy, switch to gathering information.**
> *Okay. gathering information is active and modeling is inactive.*

## stop activity

> **Dizzy, I'm done gathering information.**
> *Okay, gathering information is deactivated.*

## stop inactive activity

> **Dizzy, stop modeling.**
> *Modeling was already inactive. Right now, only gathering information is active.*

<a id="key-task-3"></a>[back to top](#)

# stop tracking

> **Dizzy, stop tracking.**
> *Okay, I've stopped tracking for portfolio. Do you want to hear a summary of your session?*
> **No thanks.**

> **Dizzy, stop tracking.**
> *Okay, I've stopped tracking for portfolio. Do you want to hear a summary of your session?*
> **Sure.**
> *In total, you worked for 1 hour and 21 minutes, and activities you spent the most time on were modeling and evaluation. You didn't spend any time on problem definition or communication.*

The user can also ask a specific question instead of requesting the summary.

> **Dizzy, stop tracking.**
> *Okay, I've stopped tracking for portfolio. Do you want to hear a summary of your session?*
> **How long did I spend modeling?**
> *This session, you spent 32 minutes on modeling, which is 40 percent of the session time. Over the whole project, you've spent 4 hours and 41 minutes on modeling, which is 32 percent of your total project time.*

The user could continue to ask another question if desired.

<a id="key-task-4"></a>[back to top](#)

# manage projects

## create projects

> **Dizzy, start a new project.**
> *Sure. What should I call it?*
> **Prototyping process blog.**
> *Okay, I've created the project prototyping process blog. Do you want to start tracking now?*
> **Yes!**
> *Alright, I've started tracking for prototyping process blog.*

## get recent project

> **Dizzy, what's my most recent project?**
> *The last project you worked on was capstone.*

The assistant can use the context from the previous responses to perform actions on this project, such as starting tracking or querying activity data.

> **Start tracking that.**
> *Okay, I've started tracking for capstone.*

<a id="key-task-5"></a>[back to top](#)

# query activity data

To query activity data for a project, the user will need to first select a project:

> **Dizzy, what's my most recent project**
> *The last project you worked on was capstone.*
> **How am I doing?**
> *Across 16 sessions, you've worked on capstone for a total of 14 hours and 31 minutes. You've spent the most time on modeling and the least time on feasibility analysis and decision.*

> **Dizzy, tell me about capstone.**
> *Across 16 sessions, you've worked on capstone for a total of 14 hours and 31 minutes. You've spent the most time on modeling and the least time on feasibility analysis and decision.*

The user can ask the assistant follow-up questions for more information, such as:

> **How much time have I spent on modeling?**
> *You've spent 4 hours and 41 minutes on modeling, which is 32 percent of your total project time.*

> **How long was my longest session?**
> *Your longest session in capstone was 3 hours and 29 minutes, on February 16th.*

</div>