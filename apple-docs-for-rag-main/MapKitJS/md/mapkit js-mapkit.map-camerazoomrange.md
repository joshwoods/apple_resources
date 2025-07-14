

- MapKit JS
- mapkit.Map
-  cameraZoomRange 

Instance Property

# cameraZoomRange

The minimum and maximum distances of the camera from the map center.

MapKit JS 5.23+

``` source
attribute mapkit.CameraZoomRange cameraZoomRange;
```

## Mentioned in 

MapKit JS 5

## Discussion

Get or set this property with a mapkit.CameraZoomRange instance, which is an object containing minCameraDistance and maxCameraDistance properties.

## Topics

### Defining a Zoom Range

CameraZoomRangeLiteral

An object literal containing minimum and maximum camera distance in meters.

## See Also

### Manipulating the visible portion of the map

center

The map coordinate at the center of the map view.

setCenterAnimated

Centers the map to the provided coordinate, with optional animation.

region

The area the map is displaying.

setRegionAnimated

Changes the map’s region to the provided region, with optional animation.

rotation

The map’s rotation, in degrees.

setRotationAnimated

Changes the map’s rotation setting to the number of specified degrees.

visibleMapRect

The visible area of the map, in map units.

setVisibleMapRectAnimated

Changes the map’s visible map rectangle to the specified map rectangle.

cameraBoundary

A constraint of the location of the center of the map.

setCameraBoundaryAnimated

Changes the map’s camera boundary with an animated transition.

cameraDistance

The altitude of the camera relative to the elevation of the center of the map.

setCameraDistanceAnimated

Changes the map’s camera distance with an animated transition.

setCameraZoomRangeAnimated

Changes the map’s camera zoom range with an animated transition.

