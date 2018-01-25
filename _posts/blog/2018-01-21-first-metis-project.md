---
layout: article
title: "An Analysis of NYC Subway Usage"
categories: blog
excerpt: "My first project for Metis - an analysis of NYC subway traffic"
tags: [blog, metis]
image:
  feature: nyc-subway2.jpg
  teaser: nyc-subway-teaser2.jpg
  credit: Martin David 
  creditlink: https://unsplash.com/photos/vClkunKSKkw?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText
---

I recently quit my job as the Senior Business Analyst at [Sittercity](https://www.sittercity.com/) to take a full-time, three month data science course with [Metis](https://www.thisismetis.com/). Read more about my experience with Metis here. 

At Metis we hit the ground running and were assigned our first of five projects on the very first day. The purpose of this exploratory analytics project was to give us greater experience in python, particularly with Pandas, Numpy and Matplotlib.

___

## Project - Analysis of NYC Subway Commuter Traffic

This first project imagines that we are contacted by a potential client, WomenTechWomenYes, to solicit our help optimizing their street team work to collect the most emails from NYC commuters entering subway stations around the city. 

<div id="awesome">
	<blockquote>
		
		<p><font size="3">WomenTechWomenYes (WTWY) has an annual gala at the beginning of the summer each year. As we are new and inclusive organization, we try to do double duty with the gala both to fill our event space with individuals passionate about increasing the participation of women in technology, and to concurrently build awareness and reach.		</font>
		</p>

		<p><font size="3">To this end we place street teams at entrances to subway stations. The street teams collect email addresses and those who sign up are sent free tickets to our gala.
			</font>
		</p>

		<p><font size="3">Where we’d like to solicit your engagement is to use MTA subway data, which as I’m sure you know is available freely from the city, to <b>help us optimize the placement of our street teams, such that we can gather the most signatures, ideally from those who will attend the gala and contribute to our cause</b>.
		</font>
		</p>
	</blockquote>
</div>


Clearly the goal of this new organization is to **build awareness**, and they're hoping to achieve that goal by 1) connecting with as many commuters as possible and 2) specifically targeting individuals who are most likely to attend their gala and contribute to their cause. 

Ideally, we would conduct an analysis of the NYC transit system and surrounding areas that would satisfy both objectives by identifying:

**1) The Most Frequented Stations** - The station locations with the highest number of commuters

**2) At Optimized Times** - The times when these stations are most frequented

**3) In Ideal Areas** - The stations in areas most densely populated with tech companies and households likely to donate to non-profit organizations

___

## Enter... the Triple Constraint

There is a concept in project management that a project's quality is constrained by time, resources and scope:

 <center><figure>
	<img src="http://ptgmedia.pearsoncmg.com/images/intro_9780133839753/elementLinks/01fig01.jpg" alt="">
</figure></center>

Because our time and resources were fixed, we decided to limit the scope of our project to avoid producing low quality results.

In the end, our goal was to accomplish two things:

> **Our goal is to identify:**

> 1) The Most Frequented Stations

> 2) At Optimized Times

___

## Data and Methodology

We were able to pull data directly from the MTA website to get weekly counts of turnstile rotations from each subway station and also a file for subway station location data. There were some limitations here:

- The turnstile rotation counts are sampled at irregular intervals (approximately every four hours)
- The turnstile rotation counts will randomly turn over and start counting backwards
- There is no way to directly link turnstiles to station locations

___

## Results

I put together an interactive dashboard, hosted on Tableau Public, to visualize the results of our analysis and enable exploration of optimal locations for specific periods of time during the months our client would be canvassing.

Click on an element in the bar chart or map below to view the times most optimal for a given location or hover over a specific time period to view the station with the greatest number of average commuter entries during that interval.

Feel free to explore below or view this dashboard directly on my [Tableau Public](https://public.tableau.com/profile/tiffany.moeller#!/vizhome/MTA-Entry-Traffic-Dash/StationLocationsandTimes) profile!

<center><iframe src="https://public.tableau.com/views/MTA-Entry-Traffic-Dash/StationLocationsandTimes?:showVizHome=no&:embed=true" width="1020" height="900" frameborder="0"></iframe></center>
 
