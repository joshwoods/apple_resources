

- MapKit JS
- mapkit.Map
-  cameraBoundary 

Instance Property

# cameraBoundary

A constraint of the location of the center of the map.

MapKit JS 5.23+

``` source
attribute CameraBoundaryDescription cameraBoundary;
```

## Return Value

An object containing both mapkit.CoordinateRegion and mapkit.MapRect instances.

## Mentioned in 

MapKit JS 5

## Discussion

Setting this property requires either a mapkit.CoordinateRegion or a mapkit.MapRect instance as a value. Getting the property returns an object containing both mapkit.CoordinateRegion and mapkit.MapRect instances.

## Topics

### Defining a Camera Boundary

CameraBoundaryDescription

An object literal containing at least one property defining an area on the map.

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

setCameraBoundaryAnimated

Changes the map’s camera boundary with an animated transition.

cameraDistance

The altitude of the camera relative to the elevation of the center of the map.

setCameraDistanceAnimated

Changes the map’s camera distance with an animated transition.

cameraZoomRange

The minimum and maximum distances of the camera from the map center.

setCameraZoomRangeAnimated

Changes the map’s camera zoom range with an animated transition.

