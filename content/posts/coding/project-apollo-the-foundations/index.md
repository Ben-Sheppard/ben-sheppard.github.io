---
title: "Project Apollo: The foundations"
date: 2024-03-04T21:19:52Z
categories: ["coding"]
tags: ["apollo", "software", "development", "music", "detection"]
draft: true
---

For a while now I've found myself often sharing songs with friends at a particular timestamp because I really like the way that it sounds. It's often a specific riff that evokes a particular feeling or allows me to process a feeling.

I've been thinking about how I could craft something that you could feed a section of a song into and it would suggest songs that have similar riffs or sounds. I realise that this is likely something that is already happening in apps such as Spotify or Apple Music in some form, but I think it would be a fun project to work on regardless!

### The Plan

I'm going to call this project Apollo, after the Greek god of music, and I'm going to document my progress here. My first thoughts are that I need:
1. A way to feed a specific section of a song into a program
2. A way to analyse the sound of that section
3. A way to compare that sound to other songs
4. A way to suggest songs that have similar sounds

It seems fairly simple listed like that, but I'm sure there will be some challenges along the way. Speaking of challenges, I am going to set out some rules for this challenge project, they are:
1. Library usage is limited to the following:
    - Standard libraries (none that abstract the actual logic away, I want to learn something here!)
    - Libraries that are used for testing
2. The algorithm should be performant
3. The storage method should be simple and easy to understand

### Step 1: Creating a base application

I'm a Java dev and I would like these projects to further and deepen my knowledge of Java also, so I'm going to use Java here!