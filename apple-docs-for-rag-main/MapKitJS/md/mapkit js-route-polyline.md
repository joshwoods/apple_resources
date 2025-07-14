

- MapKit JS
- Route
-  polyline 

Instance Property

# polyline

An instance of a polyline overlay that represents the path of a route.

MapKit JS 5.4+

``` source
attribute mapkit.PolylineOverlay polyline;
```

## Mentioned in 

MapKit JS 5

## Discussion

You can add the value of the `polyline` property directly to the map.

```
var route = directions.route({
    origin: new mapkit.Coordinate(37.616934, -122.383790),
    destination: new mapkit.Coordinate(37.3349, -122.0090201)
}, function(error, data) {

    var polylines = data.routes.map(function(route) {
        return route.polyline;
    });

    map.showItems(polylines);

});
```

## See Also

### Route geometry

path

An array of coordinate objects representing the path of the route.

Deprecated

