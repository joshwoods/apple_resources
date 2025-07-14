

- MapKit JS
-  CameraBoundaryDescription 

Structure

# CameraBoundaryDescription

An object literal containing at least one property defining an area on the map.

MapKit JS 5.23+

``` source
dictionary CameraBoundaryDescription {
 mapkit.MapRect mapRect;
 mapkit.CoordinateRegion region;
};
```

## Overview

The `CameraBoundaryDescription` can contain the `mapRect` or `region` properties, or both. Both properties describe a rectangular area on the map.

## Topics

### Defining a Camera Boundary

mapRect

A rectangular area on a two-dimensional map projection.

region

A rectangular area on a map, defined by coordinates of the rectangle’s northeast and southwest corners.

