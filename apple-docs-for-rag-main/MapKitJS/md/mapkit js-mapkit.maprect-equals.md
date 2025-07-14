

- MapKit JS
- mapkit.MapRect
-  equals 

Instance Method

# equals

Compares whether two map rectangles are equal.

MapKit JS 5.0+

``` source
boolean equals(
 mapkit.MapRect anotherRect
);
```

## Parameters 

`anotherRect`  

The map rectangle to use for comparison.

## Return Value

Returns `true` if a rectangle exactly matches `anotherRect`. Returns `false` if the origin point or size values are different.

## See Also

### Working with map rectangles

copy

Returns a copy of a map rectangle.

scale

Returns a scaled map rectangle for a map location.

toCoordinateRegion

Returns the region that corresponds to a map rectangle.

