

- MapKit JS
- mapkit.MapPoint
-  equals 

Instance Method

# equals

Indicates whether two map points are equal.

MapKit JS 5.0+

``` source
boolean equals(
 mapkit.MapPoint anotherPoint
);
```

## Parameters 

`anotherPoint`  

A map location to use for comparison.

## Return Value

Returns `true` if the `x` and `y` values of the map point exactly match the corresponding values of `anotherPoint`. Returns `false` if the values aren’t an exact match.

## See Also

### Working with map points

copy

Returns a copy of the location.

toCoordinate

Converts a map point into a coordinate with latitude and longitude.

