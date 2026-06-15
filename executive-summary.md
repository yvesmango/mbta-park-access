# Executive Summary

## The question

As Boston prepared for World Cup attention and the increased scrutiny that comes with a global event, we asked a simple equity question: how easy is it for people to reach parks from MBTA stations on foot?

## What we measured

We measured walking access using network-based isochrones at 5, 10, and 15 minutes, assuming a pedestrian speed of 4.5 km/h. The goal was to estimate how much of the MBTA system can reach a park within a realistic walk rather than a straight-line radius.

## Data sources

This analysis combines three main inputs: MBTA station data, MassGIS DCR open space, and pedestrian network data from OpenStreetMaps.

## Key findings

The headline result is strong: 98.6% of MBTA stations reach a park within a 15-minute walk. Only 2 stations appear to have no access in the measured bands, while the Green Line E branch stands out as the gold standard for park access.

## Methodology note

We used network-buffered isochrones rather than convex hulls. That distinction matters because convex hulls can overstate access by filling in areas people cannot actually walk through. The network approach follows the spirit of Kuan Butts' work on pedestrian accessibility, which prioritizes real walkable paths over simplified geometry.

## So what?

The practical takeaway is clear: the system is already performing well overall, but targeted pedestrian improvements at the 2 outlier stations could close the remaining gap.

## Limitations

This analysis depends on the completeness of OSM pedestrian data, which may miss informal or newly built paths. It also measures access to parks, not park quality, size, amenities, or safety.
