

- MapKit JS
- mapkit.Map
-  isRotationEnabled 

Instance Property

# isRotationEnabled

A Boolean value that determines whether the user may rotate the map using the compass control or a rotate gesture.

MapKit JS 5.0+

``` source
attribute boolean isRotationEnabled;
```

## Discussion

When `isRotationEnabled` is `false`, you can still rotate the map programmatically by using rotation or setRotationAnimated.

## See Also

### Accessing interaction properties

isRotationAvailable

A Boolean value that indicates whether map rotation is available.

isScrollEnabled

A Boolean value that determines whether the user can cause the map to scroll with a pointing device or with gestures on a touchscreen.

isZoomEnabled

A Boolean value that determines whether the user may zoom in and out on the map using pinch gestures or the zoom control.

