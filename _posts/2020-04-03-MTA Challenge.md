---
layout: post
title: Women Yes Women Tech
---

<h2>Proposal</h2>
This project addresses the question posed by the Women Yes Women Tech organization: To generate interest and awareness for an annual gala, which NYC subway stations should street teams be located at to collect email addresses for potential attendees? The event will be in early summer and people who sign up for the gala will receive free tickets.  

New York's Metropolitan Transportation Authority (MTA) provides public transportation to millions of people every year and this network records turnstile data from its stations to track usage over the past couple of years.

Data: <a href="http://web.mta.info/developers/turnstile.html">MTA Turnstile data</a>

<h2>Strategy</h2>
In order to capture a timeframe that is most representative of when outreach by street teams should be done this year, the data sets analyzed were between March 30 and April 19, 2019, giving ample time for recruiting attendees before an early summer (~June) event.  

<h3>Methodology</h3>
In this exploratory data analysis project, we used the Python Data Analysis Library, *Pandas*, to clean and sort through the MTA turnstile data. Visualizations were then done using Matplotlib.  

<h2>Initial Analyses</h2>

Top twenty stations were sorted based off cumulative entries into the subway station during this time period

![Top 20 Stations]({{sodas32.github.io}}/images/top20bar.png)

Stations that were excluded due to high tourist traffic, stations in residential areas, etc. 

![Excluded stations]({{sodas32.github.io}}/images/greyedouttop20.png)

Technology company offices are concentrated in Fidi, Soho, and Midtown. 

![Tech areas]({{sodas32.github.io}}/images/Picture1.png)

Combining this information, the recommended stations to place street teams are: 

![Recommended Stations]({{sodas32.github.io}}/images/techtop20.png)

<strong>Stations to place street teams:</strong>
<ol>
    <li>34th Street-Penn Station</li> 
    <li>Grand Central-42nd Street</li>
    <li>34th Street-Herald Square</li>
    <li>14th Street-Union Square</li>
    <li>Fulton Street</li>
    <li>42nd Street- Port Authority</li> 
    <li>59th Street Columbus</li> 
    <li>Canal Street</li>
    <li>World Trade Center (PATH)</li>
    <li>47th-50th Streets Rockefeller Center</li>
</ol>
