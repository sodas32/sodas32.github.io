---
layout: post
title: Women Yes Women Tech: Gals for the Gala
---

This project addresses the question posed by the Women Yes Women Tech organization: To generate interest and awareness for an annual gala, which NYC subway stations should street teams be located at to collect email addresses for potential attendees? The event will be in early summer and people who sign up for the gala will receive free tickets.  

New York's Metropolitan Transportation Authority (MTA) provides public transportation to millions of people every year and this network records turnstile data from its stations to track usage over the past couple of years.

Data: [MTA Turnstile data]({{http://web.mta.info/developers/turnstile.html}}) 

Strategy:
In order to capture a timeframe that is most representative of when outreach by street teams should be done, the data sets analyzed were between March 30 and April 19, 2019, giving ample time for recruting attendees before an early summer (~June) event, 

Methodology: In this exploratory data analysis project, we used the Python Data Analysis Library, *Pandas*, to clean and sort through the MTA turnstile data. Visualizations were then done using Matplotlib.  


Initial analyses: 

Top twenty stations were sorted based off cumulative entries into the subway station during this time period

![Top 20 Stations]({{sodas32.github.io}}/images/top20bar.png)

Stations that were excluded due to high tourist traffic, stations in residential areas, etc. 

![Excluded stations]({{sodas32.github.io}}/images/greyedouttop20.png)

Technology company offices are concentrated in Fidi, Soho, and Midtown. Combining this information, the recommended stations to place street teams are: 

![Recommended Stations]({{sodas32.github.io}}/images/techtop20.png)


