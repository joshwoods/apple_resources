

- MapKit JS
- mapkit.Map
-  isRotationAvailable 

Instance Property

# isRotationAvailable

A Boolean value that indicates whether map rotation is available.

MapKit JS 5.0+

``` source
attribute boolean isRotationAvailable;
```

## Discussion

MapKit JS determines whether it’s possible to rotate the map, and sets isRotationAvailable to `true` or `false`. When the value is `true`, users can rotate the map and any labels on the map remain horizontal.

The value for isRotationAvailable is:

`true`  
When the client renders the map, such as by browsers that support WebGL.

`false`  
When the Apple Maps server renders the map with a grid of image tiles, or when you implement your own tile overlays (addTileOverlay).

When `isRotationAvailable` is `false`, isRotationEnabled is always `false` and rotation is always `0`.

## See Also

### Accessing interaction properties

isRotationEnabled

A Boolean value that determines whether the user may rotate the map using the compass control or a rotate gesture.

isScrollEnabled

A Boolean value that determines whether the user can cause the map to scroll with a pointing device or with gestures on a touchscreen.

isZoomEnabled

A Boolean value that determines whether the user may zoom in and out on the map using pinch gestures or the zoom control.

