# fp-in-scala-capstone
Capstone project for the Functional Programming in Scala Specialization on Coursera

## Overview

In this project we are given temperature data from the National Center for
Environmental Information of the United States. The data consists of weather
stations located throughout the world and yearly temperature records at those
locations.

The goal of the project is to extract the temperature data and produce an
interactive and zoomable visualization of temperatures and temperature
deviations across the world, using the weather station data to interpolate for
geophraphic coordinates for which we don't have temperature data. The image
below depicts the end result.

![Project Goal](project_goal_visualization.png)

Apache Spark is employed to parallelize the task of joining temperature data with
weather station locations and computing per-year averages.

## Data

Due to size, the data is not included directly in this repo, but it can be
downloaded from [here](http://alaska.epfl.ch/files/scala-capstone-data.zip).

Once downloaded, extract the `resources` folder directly to `src/main`.

## Execution

Kick off a run with `sbt run`. You may need to set the `-mem` option to a high
value (e.g. 4096) depending on your settings.