

- MapKit JS
- mapkit.Map
-  setVisibleMapRectAnimated 

Instance Method

# setVisibleMapRectAnimated

Changes the map’s visible map rectangle to the specified map rectangle.

MapKit JS 5.0+

``` source
mapkit.Map setVisibleMapRectAnimated(
 mapkit.MapRect mapRect,
 optional boolean animate
);
```

## Parameters 

`mapRect`  

The map’s new visible area, in map units.

`animate`  

A Boolean value that determines whether MapKit JS animates the visible area change. The default value is `true`.

## Return Value

Returns the map object.

## Discussion

By default, MapKit JS animates the change.

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

