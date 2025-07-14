

- MapKit JS
-  mapkit.MapPoint 

Class

# mapkit.MapPoint

A location, in map units, of a point on the Earth’s surface projected onto a 2D map.

MapKit JS 5.0+

``` source
interface mapkit.MapPoint
```

## Overview

Map units are a value from `0` to `1` that represent an interpolated location within the height or width of the full map projection. On a two-dimensional map, the upper-left corner of the map projection has the coordinate (`0,` `0`), and the lower-right corner of the map projection has the coordinate (`1,` `1`).

As another point of reference, `mapkit.MapPoint(0.5,` `0.5)` corresponds to the center of the map, which MapKit JS also represents as the coordinate `mapkit.Coordinate(0,` `0)`.

## Topics

### Creating a map point

mapkit.MapPoint

Creates a map location.

### Defining a map point

x

The location of the map point along the map’s x-axis.

y

The location of the map point along the map’s y-axis.

### Working with map points

copy

Returns a copy of the location.

equals

Indicates whether two map points are equal.

toCoordinate

Converts a map point into a coordinate with latitude and longitude.

## See Also

### Map units

mapkit.MapRect

A rectangular region, in map units, of a two-dimensional map projection.

mapkit.MapSize

A pair of values, in map units, that define the width and height of a rectangular area of a map projection.

mapkit.CameraZoomRange

A minimum and maximum camera distance, in meters, from the center of the map.

