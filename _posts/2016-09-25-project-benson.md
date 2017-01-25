---
layout: splash
title: Project Benson
categories:
  - Post
tags:
  - jupyter notebooks
  - data exploration
  - metis
---

## Background

During the first week at Metis we hit the ground running with a group project. The core skills to practice in this exercise were data munging/exploration, presentation, and design. Tools utilized this past week included: jupyter notebooks, pandas, matplotlib, and seaborn.

## Project Benson

### Introduction

For our first project at Metis, we were tasked to collaborate in groups and produce a proposal that would leverage city foot-traffic data to solve a problem of our choosing. Focusing on the problem of advertising placement, my team proposed a strategy to implement and improve performance of an advertising campaign at NYC subway stations.

The subway system in NYC hosts millions of riders everyday with a large number of regular commuters. At associated locations, advertising is not only highly visible but also conducive to brand reinforcement. To provide focus and real world application, we identified Jet.com as an ideal representative client to pitch this project.

### Data and Strategy

As a first step, our team used MTA turnstile data ([MTA developers website](http://web.mta.info/developers/turnstile.html)) to determine foot traffic in the subway system. Total traffic by station was calculated by cumulative exit/entry during the week of Sept 10th through 17th, 2016. 

Below is a visualization of exits/entries over stations with the highest traffic.

![alt text](https://github.com/jamesmcglone/jamesmcglone.github.io/tree/master/images/top\ stations.png "Stations")

WIth this information in hand, we suggested a A/B testing strategy could be implemented across the top 30 stations by traffic. Performance of a given station would be tracked by unique promotional codes that designate where the advertisement had been viewed. Initially, such promotional codes could vary based on promotional type or content. In future iterations, this strategy could also expand to test different types of positioning (e.g. stairwells, station entrances, walls, columns) and types of media (e.g. posters, billboards, wall art, even video).

An example of differentiated promo codes:

![alt text](https://github.com/jamesmcglone/jamesmcglone.github.io/tree/master/images/promocodes.png "Promo Codes")

In order to better understand who is viewing advertisements at a given station, demographic and other location based data can further supplement our primary MTA turnstile dataset. For example, using a dataset that provided real estate valuations across the city ([Property Valuation and Assessment Data](https://data.cityofnewyork.us/Housing-Development/Property-Valuation-and-Assessment-Data/rgy2-tti8/data)), we identified more affluent residential zipcodes. Coupled with the obtained traffic data, targeted advertising can account for stations located in wealthier residential areas. With further analysis, valuations can be further specified by block or distance from a given station. Other datasets, especially regional census data, may be even more informative with regards to a given area's demographics.

Residential Unit Values Across Zipcodes 

![alt text]({{ site.baseurl }}/images/housingvalues.png "Residential Units")

