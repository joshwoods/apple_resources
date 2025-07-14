

- MapKit JS
-  mapkit.MapSize 

Class

# mapkit.MapSize

A pair of values, in map units, that define the width and height of a rectangular area of a map projection.

MapKit JS 5.0+

``` source
interface mapkit.MapSize
```

## Overview

Use a map size to represent a subset of a map projection. Map units are a value from `0` to `1` that represent an interpolated location within the height or width of the full map projection.

## Topics

### Creating a map size

mapkit.MapSize

Creates an object containing the width and height of a projected coordinate span.

### Defining a map size

height

The height of the map size in map units.

width

The width of the map size in map units.

### Copying and comparing map sizes

copy

Returns a copy of the map size object.

equals

Compares the sizes of two maps and indicates whether they’re of equal value.

## See Also

### Map units

mapkit.MapPoint

A location, in map units, of a point on the Earth’s surface projected onto a 2D map.

mapkit.MapRect

A rectangular region, in map units, of a two-dimensional map projection.

mapkit.CameraZoomRange

A minimum and maximum camera distance, in meters, from the center of the map.

