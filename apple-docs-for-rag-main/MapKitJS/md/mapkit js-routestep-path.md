

- MapKit JS
- RouteStep
-  path 

Instance Property

# path

An array of coordinate objects representing the path of the route segment.

MapKit JS 5.0+

``` source
attribute mapkit.Coordinate[] path;
```

## Discussion

An array of mapkit.Coordinate objects that traces the route segment. To render the route segment on a map, set the points property of mapkit.PolylineOverlay to this array.

