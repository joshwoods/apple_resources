

- MapKit JS
- mapkit.Map
-  region 

Instance Property

# region

The area the map is displaying.

MapKit JS 5.0+

``` source
attribute mapkit.CoordinateRegion region;
```

## Discussion

This is the area currently displayed by the map, defined with a mapkit.CoordinateRegion:

```
var center = new mapkit.Coordinate(48.8468, 2.3364),
    span = new mapkit.CoordinateSpan(0.016, 0.016),
    region = new mapkit.CoordinateRegion(center, span);
```

## See Also

### Manipulating the visible portion of the map

center

The map coordinate at the center of the map view.

setCenterAnimated

Centers the map to the provided coordinate, with optional animation.

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

cameraZoomRange

The minimum and maximum distances of the camera from the map center.

setCameraZoomRangeAnimated

Changes the map’s camera zoom range with an animated transition.

