

- MapKit JS
- mapkit.Map
-  convertPointOnPageToCoordinate 

Instance Method

# convertPointOnPageToCoordinate

Converts a point in page coordinates to the corresponding map coordinate.

MapKit JS 5.0+

``` source
mapkit.Coordinate convertPointOnPageToCoordinate(
 DOMPoint point
);
```

## Parameters 

`point`  

A point in the page’s coordinate system, such as `new DOMPoint(event.pageX, event.pageY),` when handling a mouse event.

## Return Value

A mapkit.Coordinate in the map at the provided point (DOMPoint) of the page.

## Mentioned in 

Handling map events

## See Also

### Converting map coordinates

convertCoordinateToPointOnPage

Converts a coordinate on the map to a point in the page’s coordinate system.

