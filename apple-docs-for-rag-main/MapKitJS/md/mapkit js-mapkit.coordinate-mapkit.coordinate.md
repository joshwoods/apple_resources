

- MapKit JS
- mapkit.Coordinate
-  mapkit.Coordinate 

Initializer

# mapkit.Coordinate

Creates a coordinate object with the specified latitude and longitude.

MapKit JS 5.0+

``` source
new mapkit.Coordinate(
 number latitude,
 number longitude
);
```

## Parameters 

`latitude`  

The latitude in degrees.

`longitude`  

The longitude in degrees.

## Discussion

Create a new `mapkit.Coordinate` like this:

```
var coordinate = new mapkit.Coordinate(37.415, -122.048333);    // latitude, longitude
coordinate.equals(otherCoordinate) // Returns true if otherCoordinate is at the same position (within a small margin of error).
```

