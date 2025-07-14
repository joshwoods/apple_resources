

- MapKit JS
-  mapkit.CoordinateRegion 

Class

# mapkit.CoordinateRegion

A rectangular area on a map that a center coordinate and a span define, in degrees of latitude and longitude.

MapKit JS 5.0+

``` source
interface mapkit.CoordinateRegion
```

## Mentioned in 

MapKit JS 5

## Topics

### Creating a coordinate region

mapkit.CoordinateRegion

A rectangular geographic region that centers around a latitude and longitude coordinate.

### Defining the region

center

The center point of the region.

span

The horizontal and vertical span representing the amount of map to display.

### Inspecting the region

radius

The distance provided in meters or the longest distance derived from the center point to the region’s bounding box.

### Comparing, copying, and converting regions

copy

Returns a copy of the calling coordinate region.

equals

Returns a Boolean value indicating whether two regions are equal.

toBoundingRegion

Returns the bounding region that corresponds to the specified coordinate region.

toMapRect

Returns the map rectangle that corresponds to the calling coordinate region.

## See Also

### Map coordinates

mapkit.Coordinate

An object representing the latitude and longitude for a point on the Earth’s surface.

mapkit.CoordinateSpan

The width and height of a map region.

mapkit.BoundingRegion

A rectangular area on a map, which coordinates of the rectangle’s northeast and southwest corners define.

