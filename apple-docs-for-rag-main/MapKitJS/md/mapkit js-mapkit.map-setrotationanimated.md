

- MapKit JS
- mapkit.Map
-  setRotationAnimated 

Instance Method

# setRotationAnimated

Changes the map’s rotation setting to the number of specified degrees.

MapKit JS 5.0+

``` source
mapkit.Map setRotationAnimated(
 number degrees,
 optional boolean animate
);
```

## Parameters 

`degrees`  

The map’s rotation, in degrees.

`animate`  

A Boolean value that determines whether the rotation change animates. The default value is `true`.

## Return Value

Returns the map object.

## Discussion

By default, MapKit JS animates the rotation change. This function changes the map’s rotation even if isRotationEnabled is `false`.

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

cameraZoomRange

The minimum and maximum distances of the camera from the map center.

setCameraZoomRangeAnimated

Changes the map’s camera zoom range with an animated transition.

