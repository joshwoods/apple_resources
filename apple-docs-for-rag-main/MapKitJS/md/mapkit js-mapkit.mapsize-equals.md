

- MapKit JS
- mapkit.MapSize
-  equals 

Instance Method

# equals

Compares the sizes of two maps and indicates whether they’re of equal value.

MapKit JS 5.0+

``` source
boolean equals(
 mapkit.MapSize anotherSize
);
```

## Parameters 

`anotherSize`  

The map size to use for comparison.

## Return Value

Returns `true` if the `width` and `height` values of a map size exactly match the corresponding values of `anotherSize`. Returns `false` if the values aren’t an exact match.

## See Also

### Copying and comparing map sizes

copy

Returns a copy of the map size object.

