

- MapKit JS
- mapkit.Map
-  isZoomEnabled 

Instance Property

# isZoomEnabled

A Boolean value that determines whether the user may zoom in and out on the map using pinch gestures or the zoom control.

MapKit JS 5.0+

``` source
attribute boolean isZoomEnabled;
```

## Discussion

Pinch-to-zoom with a trackpad requires browser touch event support. You can zoom the map programmatically when zoom isn’t in an enabled state by changing the region or visibleMapRect.

## See Also

### Accessing interaction properties

isRotationAvailable

A Boolean value that indicates whether map rotation is available.

isRotationEnabled

A Boolean value that determines whether the user may rotate the map using the compass control or a rotate gesture.

isScrollEnabled

A Boolean value that determines whether the user can cause the map to scroll with a pointing device or with gestures on a touchscreen.

