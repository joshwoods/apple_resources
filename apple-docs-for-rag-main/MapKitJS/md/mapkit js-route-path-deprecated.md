

- MapKit JS
- Route
-  path Deprecated

Instance Property

# path

An array of coordinate objects representing the path of the route.

MapKit JS 5.0–5.4Deprecated

``` source
attribute mapkit.Coordinate[][] path;
```

Deprecated

Use polyline instead of path.

## Discussion

An array of coordinates that reflect the complete path of the route, including all of its steps. To render this route on a map, set the points property of a mapkit.PolylineOverlay to this array.

## See Also

### Route geometry

polyline

An instance of a polyline overlay that represents the path of a route.

