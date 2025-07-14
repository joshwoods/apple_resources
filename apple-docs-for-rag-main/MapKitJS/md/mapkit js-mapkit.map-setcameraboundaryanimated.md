

- MapKit JS
- mapkit.Map
-  setCameraBoundaryAnimated 

Instance Method

# setCameraBoundaryAnimated

Changes the map’s camera boundary with an animated transition.

MapKit JS 5.23+

``` source
mapkit.Map setCameraBoundaryAnimated(
 mapkit.CoordinateRegion coordinateRegion,
 |mapkit.MapRect mapRect,
 optional boolean animate
);
```

## Parameters 

`mapRect`  

This can be an instance of mapkit.CoordinateRegion or mapkit.MapRect.

`animate`  

A Boolean value that determines whether MapKit JS animates the visible area change. The default value is `true`.

## Return Value

Returns the map object.

## Mentioned in 

MapKit JS 5

## Discussion

By default, the change of boundary animates.

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

cameraDistance

The altitude of the camera relative to the elevation of the center of the map.

setCameraDistanceAnimated

Changes the map’s camera distance with an animated transition.

cameraZoomRange

The minimum and maximum distances of the camera from the map center.

setCameraZoomRangeAnimated

Changes the map’s camera zoom range with an animated transition.

