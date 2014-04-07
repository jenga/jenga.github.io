---
layout: post
title: "There is nothing new under the sun"
date: 2014-03-25 16:35:00
tags:
- generalist
- multidisciplinary
- data analysis
---

There is something to be said for exposing yourself to different industries, as everyone has a different view of how to the same things. Let's take data analysis as an example (of course!). When I think about how most people perform data analysis with electrophysiology traces, I pictured proprietary file formats examined in either proprietary software or home-grown MATLAB analysis scripts. Keep in mind that this is time series data.

At this moment, I have some heavy metal music streaming out of my laptop speakers. Guess what music is? Time-series data. Like electrophysiology traces, it has regions of interests (usually quantized to bars of music). It has distinct features - properly filtered, that hard snare probably sounds looks alot like an action potential! Now the music industry has a unique way of working with their data because they view their data analysis process as a creative process. Sections of tracks are defined, and then mixed against each other, put into different orders. Individual tracks are put through a variety of filters and postcapture processing to create a unique sound.

How is this different from our research process? We collect recordings - some are good, some are bad. Of the good ones, we identify our sections of interest, put the data through filters, group them together and, instead of a melody with a kickass baseline, we get some pretty histograms and plots. 

The main difference is in the flow of the tools we use. There are many different recording software suites, certainly, and each has a slighly different way of approaching the composition of music. But the end product is the same. And while the workflow is different in each, they use the same steps of analysis - acquire, sort, process, compile.

What we need in electrophysiology is a similar workflow to what has been defined in the music recording industry - a recording interface with plugins, modules, visual drag-and-drop. Composing multiple recordings on top of each other. Each track is, instead, a cell. Each cell has multiple recordings, but we can select which is the best. Metainformation about the "track" is embedded with the data.

So what's the current issue with scientific tools? We rely on two things mainly: our lab books and our analysis software - never the two shall meet. The lab book is probablematic. It relies on a linear temporal model, without appropriate grouping of data into experiments or concepts. This is not how science works. 
