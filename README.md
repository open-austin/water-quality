# Austin Creeks Water Quality

### The problem:
It is hard to know when swimming spots and other recreational areas are dangerous to health because of bacteria or other safety hazards.

Here is a link to the original [project proposal](https://github.com/open-austin/project-ideas/issues/74).

_This is an infant project._ 

**[Create an issue](https://github.com/open-austin/water-quality/issues/new) if you have ideas and comment on any [open issues](https://github.com/open-austin/water-quality/issues/) if you have interest in contributing.**

## Potential Application Architecture

These smaller pieces could be seperate services or part of one application that does the whole thing. Here are some ideas:

1. An analyzer/scoring program that runs through the public data and scores each site/creek. It looks like that might be hard to do that as you pointed out the measurement type for E Coli counts in varying units. I'm thinking what would be nice is if the program was able to automatically:
  - download the input data from the City's data portal
  - evaluate each site and/or creek and give it some score or color assignment based on the safety of the water.
  - print out the scores in a new table
3. An API that you can query for each creek's score.
2. A twitter bot that queries the API and runs logic based on each creek and decides what to tweet out.
3. A web app/visualization that lets you see the results of the output table based on a map of the waterways and/or a list of creeks you can filter/sort.
