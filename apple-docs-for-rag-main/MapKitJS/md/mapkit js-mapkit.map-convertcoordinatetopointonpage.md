

- MapKit JS
- mapkit.Map
-  convertCoordinateToPointOnPage 

Instance Method

# convertCoordinateToPointOnPage

Converts a coordinate on the map to a point in the page’s coordinate system.

MapKit JS 5.0+

``` source
DOMPoint convertCoordinateToPointOnPage(
 mapkit.Coordinate coordinate
);
```

## Parameters 

`coordinate`  

The coordinate that displays on the map.

## Return Value

A DOMPoint in the page coordinates that corresponds to the provided map `coordinate`.

## See Also

### Converting map coordinates

convertPointOnPageToCoordinate

Converts a point in page coordinates to the corresponding map coordinate.

