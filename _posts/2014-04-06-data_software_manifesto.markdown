---
layout: post
title: Data Software Manifesto
date: 2014-04-06 15:13:00
tags:
 - software development
 - data
---

The core concepts for creating data analysis software are:

1. Reproducible
2. Accurate
3. Responsive
4. Auditable
5. Collaborative

# Reproducible

## Why it is important
Recent publications have brought to light concerns about the reproducibility of experiments in from publications. These are justifiable concerns, as major findings should be reproducible in within multiple settings. However, beyond just recreating a verifying results, data analysis methods and procedures should also be reproducible. For now, we rely on generally vague descriptions in Methods and Materials sections to allow others to replicate our results. However, if a researcher were to give you there data today, I still doubt that you could reproduce their analyses. This is not because I believe these people to be deceitful or even incorrect, but because the vast numbers of parameters and undocumented assumptions that went into their analysis will prevent you from ever duplicating their exact output. 

Analysis should instead be as precisely documented as experiments. When scripts are used instead of point-and-click tools, there is a type of self-documentation. However, this is often not enough, as scripts evolve over time, while figures and tables remain static unless meticulously updated and kept in sync. Which version of your script did you use to analyse the data for that graph? What were the parameters for the high-pass filter you used to clean that time-series?

> Analysis should be as precisely documented as experiments

## Key building blocks
All analysis should be done using scripts of software that allow for propogation of change throughout all results of analyses. Adjustments to data should automatically force reanalysis, changes to analysis should update results whereever they live. Analyses and results should be versioned to keep things in sync.

# Accurate

## Why it is important
There is arguable nothing more important than the accuracy of analyses. Whether code is written in FORTRAN or Julia, or analyses performed in Stata or by hand, if they are not accurate, they are useless and dangerous. However, if a postdoc writes analysis code in a lab, who review it to ensure it is accurate? We assume that the postdoc knows enough to write analysis code that can perform complex operations and yet return correct results, all without code review or even sober second though. Test-driven development is relegated to the software development world, and is, based on my own experience, rarely used within day-to-day scientific programming.

> If analyses are not accurate, they are useless and, potentially, dangerous

## Key building blocks
All analysis code should be reviewed by the community. Bugs should be reported and hotfixes merged for rapid distribution to all users of the analysis code. No code should used unless it has been at least examined by a second code reviewer. Test-driven development processes should be used to ensure that changes do not compromise the accuracy of the code. Statically-typed languages should be preferred over dynamic languages, as confidence in results should be preferred over rapid code development. 

# Responsive

## Why it is important
While it is often thought that analysis is carefully planned and perfectly executed the first time, in practice, it is an iterative process that often changes over time. However, most of the components of analysis are decoupled in a traditional context. Data files are not coupled to analysis, which may take place in a standalone program like Excel or Origin, statistical tests are not coupled to analysis results, and results are not coupled to figures or tables. This means that changes to data do not cause changes to the extracted features, changes in values do not result in changes to statistical outcomes or the final figures and tables. Instead, these generally have to be manually changed, assuming that parameters can be remembered.

> Updates to data requires manual process, when it should be automatic

## Key building blocks
	

















