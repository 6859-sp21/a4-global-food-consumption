---
layout: misc
title: About
---

This is the page for the 6.859 Assignment 4. Our team is: Aik Jun Tan, Franklin Morgan, and Daniel Schwalbe-Koda.

## Overview

Our team--comprised of Aik Jun Tan, Franklin Morgan, and Daniel Schwalbe-Koda--chose to focus our project on visualizing sources of greenhouse gas emissions. The goals of our visualization are to better understand the extent and impact of meat consumption on greenhouse gas emissions, as well as to explore the effects of reducing that consumption over time. Visualizations at both the global- and country-level allow readers to compare behavior both across and within countries. We hope that readers will be able to learn more about the impact of meat consumption on greenhouse gas emissions, and to understand how their own consumption may contribute to these data.

## Sources

This visualization utilizes data from three sources: 

 - [OECD](https://data.oecd.org/agroutput/meat-consumption.htm): The OECD provides average meat consumption (kg/capita) by country for years 1990 through 2018. The consumption data are split by type of meat, and include beef, poultry, pig and sheep. It is important to note that not every country is represented, including the OECD countries themselves. However, the countries included provide important information on high-level trends and country-specific information.
- [Our World in Data](https://ourworldindata.org/food-choice-vs-eating-local): This source provided helpful context on greenhouse gas emissions in addition to data quantifying the amount of carbon emissions per kg of meat type consumed. We used this information to generate graphs of carbon emissions resulting from meat consumption--both per capita and in absolute values by country.
- [US Environmental Protection Agency](https://www.epa.gov/greenvehicles/greenhouse-gas-emissions-typical-passenger-vehicle): This final source was used to relate the impact of meat consumption to comparable effects from other sources of carbon emissions. For the purposes of this visualization, used data on passenger vehicle emissions to draw comparisons between the impact of driving a car versus eating meat.

In addition to these direct data sources, we drew inspiration for our project from previous visualizations and class examples. In learning how to utilize D3.js, the [D3 Gallery on Observable](https://observablehq.com/@d3/gallery) was incredibly useful for exploring a wide range of possibilities and for building our visualizations off of existing prototypes. We worked specifically from charts such as the [stacked area chart](https://observablehq.com/@d3/stacked-area-chart) and a recreation of [Hans Rosling's *The Wealth and Health of Nations*](https://observablehq.com/@mbostock/the-wealth-health-of-nations). The webpage template was built with Jekyll using the [Millenial theme](https://github.com/lenpaul/Millennial)


## Design Decisions

Our visualization is comprised of three charts and a dialog box. Our initial development focused on the top two charts, which are stacked area graphs showing the total meat consumption and total emissions, by meat type, for a given country over time. On the right, readers can interact with these graphs by changing the country and using the sliders to see the impact of reducing types of meat consumption beginning in a specific year.

We felt that the stacked area graph would allow readers to view both total meat consumption and meat consumption by type within a single chart. It is interesting to toggle between countries, as some--like the United States--have maintained relatively constant behaviors over time while others--like Indonesia--display massive changes in the types and amounts of meat consumed over the 30 year period. Interactions between the sliders and charts occur automatically, allowing readers to quickly explore many options and see the impact of their proposed changes. Finally, we chose to label and color the sliders to align with the type of meat they affect. This should make it easy for readers to understand how a slider will impact the associated charts.

The bottom section of our project provides a high-level comparison of countries from around the world. This visualization was a result of feedback received during class, during which classmates suggested that directly comparing the consumption and emissions across countries would be valuable. We considered multiple options for this visualization, including small multiples or a 1D scatter plot. For our final submission, however, we settled on a scatter plot showing the total emissions per country versus the average meat consumption per capita per country. The size of each country is a factor of it's population, and the color relates to the region of the world in which the country resides. Clicking on the legend will allow readers to isolate countries from a specific region. Mousing over the dots provides readers with the relevant country name, and clicking on a dot will change the top two graphs to the relevant country.

The final aspect of our visualization is the text box in the bottom right-hand corner of the screen. Our goal in including this box was to quantify the total impact of any proposed changes and to frame these numbers in a way that would resonate with readers. Based on feedback from the class, we included both the absolute drop in emissions and the same number as a percentage of the total world emissions. We also compared both of these numbers to the equivalent number of cars needed to generate the same amount of carbon emissions over a year. Finally, we framed the suggested reduction in meat consumption as a daily amount, which may feel much more tangible and attainable to readers. 

## Development Process

Our development project was very collaborative and iterative over the course of the assignment. Our team met bi-weekly to brainstorm ideas, review our progress, and divide up next steps. After selecting our dataset, each teammate spent time creating some initial visualizations within Observable workbooks. We then met to review ideas, begin combining these ideas into a a single workbook, and develop a plan for a minimum viable product. With some initial working interactions in Observable, we formatted our work to function within a website format and began editing the project website via Github. 

The process of working individually to develop ideas, then coming together to review and further brainstorm continued through the rest of the project as we incorporated feedback from classmates and developed the final version. In making decisions on what to include, we weighed the value to the reader of each visual or interactive aspect against the time expected to achieve that aspect. We are pleased with our final submission, which provides multiple opportunities for interaction and exploration of the main dataset.

In addition to attending meetings to compare work and brainstorm new ideas, each team member contributed in the following way: 
- Aik Jun (AJ) generated many of the graphs and interactions that make up our final submission, including the year and meat-type sliders, the country scatter plot, and the interaction between the scatter plot and stacked area charts. AJ also completed much of the work needed to convert our Observable code to html format.
- Franklin created some of the initial chart elements, such as the stacked bar graphs and the country selector. She also completed the MVP video and the writeup.
- Daniel did much of the work to create and update the website. He also created the textbox comparing emissions from meat consumption to those from driving cars, and added text guidance, chart formatting, and additional interactions to both the MVP and final submission. 

This assignment took a significant amount of time, as we both familiarized ourselves with D3.js and explored the opportunities for visualizing the global meat consumption dataset. Each team member spent between 20-30 hours total on this project. Some of the most time-consuming steps included translating visualizations between Observable, HTML and D3.js, and developing the additional interactions and visualizations beyond the MVP.

