

- MapKit JS
- mapkit.CoordinateRegion
-  equals 

Instance Method

# equals

Returns a Boolean value indicating whether two regions are equal.

MapKit JS 5.0+

``` source
boolean equals(
 mapkit.CoordinateRegion anotherRegion
);
```

## Parameters 

`anotherRegion`  

The region to compare.

## Return Value

`true` if the region that `anotherRegion` specifies is equal to the calling mapkit.CoordinateRegion; otherwise, `false`.

## Discussion

The following example shows how to determine whether a given region is equal to the region that’s displaying on the map.

```
// Create a map.
var map = new mapkit.Map("my-map-element-id");

// Create a region named myRegion.
var coordinate = new mapkit.Coordinate(37.415, -122.048333); // latitude, longitude
var span = new mapkit.CoordinateSpan(.016, .016); // latitude delta, longitude delta
var myRegion = new mapkit.CoordinateRegion(coordinate, span);

// Check whether myRegion is equal to the current map region.
if (myRegion.equals(map.region))
   console.log("These two regions are equal.");

```

## See Also

### Comparing, copying, and converting regions

copy

Returns a copy of the calling coordinate region.

toBoundingRegion

Returns the bounding region that corresponds to the specified coordinate region.

toMapRect

Returns the map rectangle that corresponds to the calling coordinate region.

