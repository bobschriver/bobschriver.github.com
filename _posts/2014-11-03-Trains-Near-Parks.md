---
layout: default
title: Trains Near Parks
categories: [project]
tags: [coding,project,train,Amtrak,national park,national forest]
---

![Trains Near Parks](/img/amtrak_header.png)

## Introduction ##

This project started when I looked at a map of Amtrak stations, and noticed how close many of them were to national parks
and national forests. I wanted to have a map with a mashup of these two geographic entities. I also wanted some information about
the distance from each national park and forest to an Amtrak station, for a hypothetical bike/train tour of national parks.

## Method ##

This project uses shapefile data from [National Atlas](http://www.nationalatlas.gov/maplayers.html), which I converted to GeoJSON
using an online tool. This data is then split into seperate GeoJSON files through a python script, one for the Amtrak station data and one for each
US Bureau (NPS, NFS, BLM) and the polygon's that represent the lands they caretake. This split data is then sent through another script
which computes the distance of each park and forest to its closest Amtrak station. All of this GeoJSON data is just put into a
Javscript variable which is loaded into Leafly.

## Results ##

Results can be viewed [here](http://www.csh.rit.edu/~schriver/amtrak-nationalparks/)

## Source ##

Source is hosted on github [here](https://github.com/bobschriver/amtrak-nationalparks)

