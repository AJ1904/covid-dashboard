# Demo Covid Dashboard

This project is built based on the tutorial available on Taipy website. https://docs.taipy.io/en/release-3.0/knowledge_base/demos

## What is Demo Covid Dashboard

[Demo Covid Dashboard](https://github.com/aj1904/covid-dashboard) is a multi-page application showing how Taipy Core and Taipy Gui can work together to build a minimalist but powerful application. This demo visualizes a Covid dataset for the year 2020. Pages shows different graphs and information on Covid. A Prediction page is also present to predict the number of death.

**Components/Controls**: 
  - Taipy GUI: selector, chart, map, toggle, CSS Style, multi-pages, layout
  - Taipy Core: datanode, pipeline, scenario

## How to run

This demo works with a Python version superior to 3.8. Install the dependencies using *requirements.txt* and run the *main.py* in the `src/` folder.

## Introduction

This demo manages multiple pages.

### Country page

The first page represents statistics on a specific country. The country can be changed as well as the way the data is displayed (either cumulative or density). It will interact with the line chart provided on this page.

The pie chart shows the repartition of cases between Confirmed, Recovered, and Deaths. 

### Map

A map can be found on this page to explore the data. Colors and sizes are dependent on the number of Deaths in this location.

### Predictions

This page lets anyone create scenarios to predict certain dates for a specific country. The user has to write a name and press the 'Create' button to create a scenario. The prediction will be created after clicking 'Submit' based on the prediction date and the country.

A list of scenarios can be found and any scenario can be selected to display their predictions.

### World page

Statistics on the World are presented on the page. A line chart and pie chart display the data. Moreover, the absolute or relative impact of Covid countries can be seen by changing the toggle between 'Absolute' and 'Relative'.