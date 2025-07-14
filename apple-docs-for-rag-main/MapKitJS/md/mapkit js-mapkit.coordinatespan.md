

- MapKit JS
-  mapkit.CoordinateSpan 

Class

# mapkit.CoordinateSpan

The width and height of a map region.

MapKit JS 5.0+

``` source
interface mapkit.CoordinateSpan
```

## Overview

You use the delta values in a coordinate span to indicate the desired zoom level of the map. Smaller delta values correspond to a higher zoom level. The *span* in this class refers to the width and height of a region, with distances as degrees of latitude and longitude.

## Topics

### Creating a coordinate span

mapkit.CoordinateSpan

Creates a new coordinate span object with the specified latitude and longitude deltas.

### Defining the span

latitudeDelta

The amount of north-to-south distance (in degrees) to display for the map region.

longitudeDelta

The amount of east-to-west distance (in degrees) to display for the map region.

### Copying and comparing spans

copy

Returns a copy of the coordinate span.

equals

Returns a Boolean value that indicates whether two spans are equal.

## See Also

### Map coordinates

mapkit.Coordinate

An object representing the latitude and longitude for a point on the Earth’s surface.

mapkit.CoordinateRegion

A rectangular area on a map that a center coordinate and a span define, in degrees of latitude and longitude.

mapkit.BoundingRegion

A rectangular area on a map, which coordinates of the rectangle’s northeast and southwest corners define.

