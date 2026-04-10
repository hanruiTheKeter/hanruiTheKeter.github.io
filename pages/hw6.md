---
layout: page
title: UFO Visualization
permalink: /hw6/
---

<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>

## Visualization 1: UFO Sightings by Country

<div id="vis1"></div>

This visualization shows the number of UFO sightings across different countries. A bar chart is used, where the x-axis represents the country and the y-axis represents the count of sightings. Color is also used to distinguish between different countries. A bar chart is appropriate here because it allows for clear comparison across categorical variables. In terms of data transformation, I grouped the dataset by the "country" column and computed the count of records for each country using pandas.

---

## Visualization 2: UFO Sightings Over Time

<div id="vis2"></div>

This visualization illustrates the trend of UFO sightings over time. A line chart is used, where the x-axis represents the year and the y-axis represents the number of sightings. The chart includes interactivity through tooltips. For data transformation, I converted the "datetime" column into a datetime format and extracted the year for grouping.

---

<script>
vegaEmbed('#vis1', '/chart1.json');
vegaEmbed('#vis2', '/chart2.json');
</script>
