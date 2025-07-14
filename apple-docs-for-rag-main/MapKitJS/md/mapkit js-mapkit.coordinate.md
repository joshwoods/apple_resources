

- MapKit JS
-  mapkit.Coordinate 

Class

# mapkit.Coordinate

An object representing the latitude and longitude for a point on the Earth’s surface.

MapKit JS 5.0+

``` source
interface mapkit.Coordinate
```

## Mentioned in 

Handling map events

## Overview

A mapkit.Coordinate is a point on a spherical representation of the Earth at a specific degree of latitude (`90` and -`90`) and longitude (`180` to -`180`) that you use to search for locations, place annotations, and other objects on the map.

## Topics

### Creating a coordinate

mapkit.Coordinate

Creates a coordinate object with the specified latitude and longitude.

### Defining the coordinates

latitude

The latitude, in degrees.

longitude

The longitude, in degrees.

### Comparing, copying, and converting coordinates

copy

Returns a copy of the coordinate.

equals

Returns a Boolean value indicating whether two coordinates are equal.

toMapPoint

Returns the map point that corresponds to the coordinate.

toUnwrappedMapPoint

Returns the unwrapped map point that corresponds to the coordinate.

## See Also

### Map coordinates

mapkit.CoordinateRegion

A rectangular area on a map that a center coordinate and a span define, in degrees of latitude and longitude.

mapkit.CoordinateSpan

The width and height of a map region.

mapkit.BoundingRegion

A rectangular area on a map, which coordinates of the rectangle’s northeast and southwest corners define.

