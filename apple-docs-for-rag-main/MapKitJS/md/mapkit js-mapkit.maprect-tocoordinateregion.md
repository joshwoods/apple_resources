

- MapKit JS
- mapkit.MapRect
-  toCoordinateRegion 

Instance Method

# toCoordinateRegion

Returns the region that corresponds to a map rectangle.

MapKit JS 5.0+

``` source
mapkit.CoordinateRegion toCoordinateRegion();
```

## Return Value

A mapkit.CoordinateRegion object that corresponds to a map rectangle.

## Discussion

It’s often easier to work with a map rectangle than a mapkit.CoordinateRegion.

The following example demonstrates how to convert a mapkit.MapRect instance to a mapkit.CoordinateRegion and back again:

```
var mapRect = new mapkit.MapRect(0.1, 0.2, 0.3, 0.4);

// Return a coordinate region with center (33.841220320476786, -90) and span (106.57400641480324, 108).
var coordinateRegion = mapRect.toCoordinateRegion();

// Return the same map rectangle as mapRect, plus or minus any floating point inaccuracies.
var newMapRect = coordinateRegion.toMapRect();
```

## See Also

### Working with map rectangles

copy

Returns a copy of a map rectangle.

equals

Compares whether two map rectangles are equal.

scale

Returns a scaled map rectangle for a map location.

