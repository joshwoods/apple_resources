

- MapKit JS
- mapkit.CameraZoomRange
-  mapkit.CameraZoomRange 

Initializer

# mapkit.CameraZoomRange

Describes the minimum and maximum camera distance in meters.

MapKit JS 5.23+

``` source
new mapkit.CameraZoomRange(
 CameraZoomRangeConstructorOptions|number minCameraDistance,
 optional number maxCameraDistance
);
```

## Discussion

Both minCameraDistance and maxCameraDistance must be greater than or equal to `0.` The minCameraDistance must be lower than or equal to the maxCameraDistance.

## See Also

### Defining a zoom range

CameraZoomRangeConstructorOptions

Initialization options for the camera zoom range.

