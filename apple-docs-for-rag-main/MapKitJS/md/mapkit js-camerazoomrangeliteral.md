

- MapKit JS
-  CameraZoomRangeLiteral 

Structure

# CameraZoomRangeLiteral

An object literal containing minimum and maximum camera distance in meters.

MapKit JS 5.23+

``` source
dictionary CameraZoomRangeLiteral {
 number minCameraDistance;
 number maxCameraDistance;
};
```

## Overview

Both `minCameraDistance` and `maxCameraDistance` must be greater than or equal to `0.` The `minCameraDistance` must be lower than or equal to the `maxCameraDistance`.

## Topics

### Setting Distance Constraints

minCameraDistance

The minimum allowed distance of the camera from the center of the map in meters.

maxCameraDistance

The maximum allowed distance of the camera from the center of the map in meters.

