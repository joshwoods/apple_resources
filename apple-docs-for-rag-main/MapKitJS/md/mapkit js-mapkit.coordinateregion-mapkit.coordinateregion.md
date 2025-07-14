

- MapKit JS
- mapkit.CoordinateRegion
-  mapkit.CoordinateRegion 

Initializer

# mapkit.CoordinateRegion

A rectangular geographic region that centers around a latitude and longitude coordinate.

MapKit JS 5.0+

``` source
new mapkit.CoordinateRegion(
 mapkit.Coordinate center,
 mapkit.CoordinateSpan span
);
```

## Parameters 

`center`  

A mapkit.Coordinate that’s the center point of the region.

`span`  

A mapkit.CoordinateSpan that represents the amount of map to display. The span also defines the current zoom level that the map object uses.

## Discussion

Create a coordinate region by passing a center coordinate and span to the constructor.

```
var coordinate = new mapkit.Coordinate(37.415, -122.048333); // latitude, longitude
var span = new mapkit.CoordinateSpan(.016, .016); // latitude delta, longitude delta
var region = new mapkit.CoordinateRegion(coordinate, span);
```

