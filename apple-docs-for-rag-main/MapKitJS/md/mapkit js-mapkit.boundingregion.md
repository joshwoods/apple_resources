

- MapKit JS
-  mapkit.BoundingRegion 

Class

# mapkit.BoundingRegion

A rectangular area on a map, which coordinates of the rectangle’s northeast and southwest corners define.

MapKit JS 5.0+

``` source
interface mapkit.BoundingRegion
```

## Overview

Similar to a mapkit.CoordinateRegion, mapkit.BoundingRegion represents a rectangular area on the 2D-projected surface. However, instead of describing a center coordinate and a span, MapKit JS defines a bounding region by the coordinates of the rectangle’s northeast and southwest corners.

## Topics

### Creating a bounding region

mapkit.BoundingRegion

Creates a rectangular bounding region, which the latitude and longitude coordinates of the rectangle’s northeast and southwest corners define.

### Defining a bounding region

eastLongitude

The east longitude of the bounding region.

northLatitude

The north latitude of the bounding region.

southLatitude

The south latitude of the bounding region.

westLongitude

The west longitude of the bounding region.

### Copying and converting regions

copy

Returns a copy of the calling bounding region.

toCoordinateRegion

Returns the coordinate region that corresponds to the calling bounding region.

## See Also

### Map coordinates

mapkit.Coordinate

An object representing the latitude and longitude for a point on the Earth’s surface.

mapkit.CoordinateRegion

A rectangular area on a map that a center coordinate and a span define, in degrees of latitude and longitude.

mapkit.CoordinateSpan

The width and height of a map region.

