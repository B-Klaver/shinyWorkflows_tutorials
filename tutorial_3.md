Shiny Workflows: Tutorial 3
================

## Pre-readings

- [Chapter 4:
  bslib](https://b-klaver.github.io/shinyWorkflows/bslib.html)

## Assignment

### 1) Create a branch from your current shiny app project to work on a bslib version

Using Git create a branch for a bslib version of your app and push this
to Gitlab

### 2) Building off of your previous shiny app, convert it to a bslib app

#### 2a) Change to using `page_navbar()`

Following the advanced example in the readings change your app to use
`page_navbar()`, `nav_panel()`, and `card()`.

- Change the top level tabs so that the first one is an introduction and
  the second is for data exploration (2 tabs total)

#### 2b) Update your sidebar

- Make the sidebar only appear on your second data exploration tab (ie.
  it’s minimized on the introduction tab)
- Create a Geography Level dropdown list (should include BC and HA
  option)
- Create a Geography selection dropdown list that only appears when HA
  is selected and includes all 5 HAs.
- Remove the button

#### 2c) Introduction tab

- Include a simple text blurb, play around with HTML, try adding in
  links or photos.

#### 2d) Data exploration tab

- Put your previous tabs for the plot and table into two side by side
  cards
- Make both cards have two tabs, one tab for a plot the other for a
  table
- For the first card keep your plot for geography the same, if you
  haven’t changed it to highcharter or plotly try doing so now. The
  table tab should have the data that is presented in the plot.
- The card for age and sex should have a filter in it that lets you
  filter for the year (should be on both the plot and table tab). The
  plot can be a bar chart with age group on the X axis, and counts on
  the Y axis, with bars for male and female side by side. The table
  should show the data shown in the plot.
- Add a tooltip to each card tab that gives a simple description of what
  that tab is showing.
- Add a button under each of the tables that allows you to download a
  csv of the data that’s used for that specific table.

#### 2e) Connect everything in the server

- Update both plots and tables based on the selected geographical region
  when it is selected.
- Update the age and sex plot and table based on the year when it is
  selected.
- Download the correct data when the download data button is pressed
- Remember to include the sidebar reactivity here as well (ie. minimized
  on the first page)

### 3) Merge your branch

Merge your bslib version with your shiny version using Git and push to
Gitlab

### 4) Readings

- [Chapter 5:
  Modularization](https://b-klaver.github.io/shinyWorkflows/modularization.html)
