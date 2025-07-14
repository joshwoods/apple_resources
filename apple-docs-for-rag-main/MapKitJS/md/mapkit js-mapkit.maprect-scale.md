

- MapKit JS
- mapkit.MapRect
-  scale 

Instance Method

# scale

Returns a scaled map rectangle for a map location.

MapKit JS 5.0+

``` source
mapkit.MapRect scale(
 number scaleFactor,
 mapkit.MapPoint scaleCenter
);
```

## Parameters 

`scaleFactor`  

The scale factor.

`scaleCenter`  

The center map point for scaling.

## Discussion

The following example demonstrates scaling a `mapkit.MapRect` instance first with a common center, and then with a common origin:

```
var mapRect = new mapkit.MapRect(0.1, 0.2, 0.3, 0.4);

// Scale a MapRect to be 2x the width and 2x the height of mapRect 
// and have the same center.
var scaledRect = mapRect.scale(2);

// Same scale but this time mapRect and scaledRectAroundOrigin 
// have the same origin rather than the same center.
var scaledRectAroundOrigin = mapRect.scale(2, new mapkit.MapPoint(mapRect.minX(), mapRect.maxX()));

```

## See Also

### Working with map rectangles

copy

Returns a copy of a map rectangle.

equals

Compares whether two map rectangles are equal.

toCoordinateRegion

Returns the region that corresponds to a map rectangle.

