

- MapKit JS
-  mapkit.MapRect 

Class

# mapkit.MapRect

A rectangular region, in map units, of a two-dimensional map projection.

MapKit JS 5.0+

``` source
interface mapkit.MapRect
```

## Overview

Use a `mapkit.MapRect` to represent a rectangular region within a map projection. Map units are a value from `0` to `1` that represent an interpolated location within the height or width of the full map projection.

## Topics

### Creating a map rectangle

mapkit.MapRect

Creates an object that represents a rectangular region of the map projection.

### Defining a map rectangle

origin

The origin point of a rectangle.

size

The width and height of a rectangle, starting from the origin point.

### Obtaining rectangle metrics

maxX

Returns the maximum x-axis value of a rectangle.

maxY

Returns the maximum y-axis value of a rectangle.

midX

Returns the midpoint along the x-axis of a rectangle.

midY

Returns the midpoint along the y-axis of a rectangle.

minX

Returns the minimum x-axis value of a rectangle.

minY

Returns the minimum y-axis value of a rectangle.

### Working with map rectangles

copy

Returns a copy of a map rectangle.

equals

Compares whether two map rectangles are equal.

scale

Returns a scaled map rectangle for a map location.

toCoordinateRegion

Returns the region that corresponds to a map rectangle.

## See Also

### Map units

mapkit.MapPoint

A location, in map units, of a point on the Earth’s surface projected onto a 2D map.

mapkit.MapSize

A pair of values, in map units, that define the width and height of a rectangular area of a map projection.

mapkit.CameraZoomRange

A minimum and maximum camera distance, in meters, from the center of the map.

