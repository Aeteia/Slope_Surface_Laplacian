# Slope_Surface_Laplacian
Quick script to determine slope surface and laplacian operator for addition to a moraine classification algorithm.

## Rationale
This script is intended to be added to https://github.com/ArcticSnow/periglacial_detection during development of the algorithm.

## What this does
1) Imports the DEM intended for K Means classification
2) Produces a low pass filter (sub 200 m).
3) Produces a slope surface from the low pass filter, thus showing general slope within the region of study rather than the slope of HF features.
4) Operates a laplacian filter of size 200 m across both the DEM and the low pass filter.
5) Writes the Slope surface and laplacian filters to geoTIFF.
