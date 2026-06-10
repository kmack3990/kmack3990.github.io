---
layout: post
title: Working with the City of Denver at CPD
date: 2026-6-10
preview: true
---

<img src="/images/cpd-denver.png" width="50%">

### My Time with the City of Denver

Since stepping into my role with Community Planning and Development at the City of Denver, I have had the opportunity to work across a wide range of projects that sit at the intersection of data engineering, analytics, and applied machine learning. What has stood out most is how deeply data can influence both day-to-day operational decisions and long-term strategic planning when it is structured, accessible, and thoughtfully communicated.

Early on, I focused heavily on building a foundation for scalable, transparent data systems that could be used across teams. One of my first major initiatives involved working with American Community Survey (ACS) data. The goal was to take highly granular demographic and socioeconomic data and transform it into a format that could be meaningfully used by planners and decision-makers across the city.

This required building a full pipeline to scrape, clean, and standardize ACS data, followed by aggregations at multiple geographic levels, including census tracts, neighborhoods, NPI-level groupings, and citywide summaries. The challenge was not just technical—it was about ensuring consistency across geographic boundaries and making the data intuitive for non-technical users. The end result was a scalable dataset that could support multiple analytical use cases and reporting needs across CPD.

That work ultimately contributed to the development of public-facing neighborhood dashboards, which translate complex datasets into accessible insights for residents, planners, and policymakers. These dashboards allow users to explore neighborhood-level trends in housing, demographics, and development activity through a centralized interface.
[Neighborhood Dashboard](https://www.denvergov.org/Community/Neighborhoods/Neighborhood-Dashboards)

Another major area of focus has been forecasting and predictive analytics. One of the most impactful projects I worked on involved modeling departmental log volumes to better understand workload distribution across teams. The objective was to forecast future demand at weekly, monthly, and yearly horizons so that teams could better anticipate staffing needs and operational capacity.
To accomplish this, I applied a combination of traditional time series approaches and machine learning techniques using Python. This included experimenting with models that could capture both trend and variability in operational data, as well as testing how different aggregation levels influenced forecast stability. The result was a forecasting framework that provided actionable insights into workload patterns and helped inform more proactive resource planning across the department.

<img src="/images/LogVolForecast.png" width="50%">

In parallel, I led the development of the Development Services Teams dashboard, which brought together multiple operational teams into a single unified analytical view for the first time. Prior to this effort, data was largely siloed across different reporting structures, making it difficult to understand cross-team performance and dependencies.
By integrating these datasets into a single Power BI dashboard, I was able to create a shared source of truth that improved visibility across teams and leadership. This dashboard has since been adopted agency-wide and is now used as a reference model for other departments seeking to build similar reporting tools. The most rewarding part of this work has been seeing it evolve from a technical build into a widely used operational asset that supports real decision-making.

<img src="/images/DSTeams.png" width="50%">

Across all of these projects, the common thread has been transformation. Transformation meaning turning fragmented or complex datasets into structured systems that people can actually use. Whether it is building scalable data pipelines, designing forecasting models, or developing enterprise dashboards, I continue to focus on creating solutions that are not only technically sound but also durable and practical in real-world government operations.
