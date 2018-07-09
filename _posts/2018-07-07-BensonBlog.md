---
layout: post
title: Week 1 @ Metis Data Science Bootcamp: Project Benson!
---

Monday 7/2/18 marked the start of the journey into Data Science with Metis.  We are a cohort of 14 people, of varying industry experience and backgrounds.  As we learned primarily about 
Pandas in Week 1, our newfound knowledge was put to the test via **Project Benson!**

# OBJECTIVES #
The objective of Project Benson was to assist a NYC based non-profit to market and get donors and attendees for their *"Women in Technology"* gala event.  Given the resource constraints of 
the non-profit, the goal of the project was to recoomend those MTA stations where a team could maximize their time to market the event and recruit donors and attendees.

# DATA #
For this project the team primarily used [MTA ridership data.](http://web.mta.info/developers/turnstile.html).  We analyzed entry data from May and June of 2018, since the gala would be 
held in June 2019.

To provide additional context the team overlaid the following information on the MTA ridership data to target those stations with exposure to women interested or working in technical 
fields:
1. Demographic data of the station localities to filter out stations with large femal populations in their locality
2. Proximity of technology focused companies to the stations
3. Demographic data showing the level of education of the population near the stations
4. Proximity of universities to the stations

# METHODOLOGY #
Our methodology, at a high level, consisted of the following steps:
1. Identify the top MTA stations by riderhsip
2. Weigh the above criteria to determine the final ranking of stations:
    - Ridership volume: 40%
    - %age of female population: 20%
    - Proximity of tech companies: 20%
    - Level of education: 15%
    - Proximity of Universities: 5%
3. Provide recommendations that can be accommodate changing constraints:
    - 2 stations with specific days of the week that will maximize the probability of attracting donors and attendees to the gala
    - 4 stations if the non-profit has a larger team to work with
    - Complete list of ranked stations if multiple teams are available to do the marketing

# CONCLUSION #
Based on our analysis, my team concluded that the non-profit concentrate on the busiest days of the week for their marketing efforts.  These days are:
**1. Tuesday**
**2. Wednesday**
**3. Thursday**

The list of stations that should be canvassed are as follows:

 Minimum Resources | More Resources | Many Resources 
 ----------------- | -------------- | -------------- 
 Grand Central Station | Grand Central Station | Grand Central Station
 Union Square Station | Union Square Station | Union Square Station
 | | 23 Street | 23 Street
 | | Penn Station | Penn Station
 | | | Herald Square
 | | | 59 Street / Lexington
