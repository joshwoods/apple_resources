

- SceneKit
- SCNBoundingVolume
-  boundingBox 

Instance Property

# boundingBox

The minimum and maximum corner points of the object’s bounding box.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
var boundingBox: (min: SCNVector3, max: SCNVector3) { get set }
```

## Discussion

Scene Kit defines a bounding box in the local coordinate space using two points identifying its corners, which implicitly determine six axis-aligned planes marking its limits. For example, if a geometry’s bounding box has the minimum corner `{-1, 0, 2}` and the maximum corner `{3, 4, 5}`, all points in the geometry’s vertex data have an x-coordinate value between `-1.0` and `3.0`, inclusive.

The coordinates provided when reading this property are valid only if the object has a volume to be measured. For a geometry containing no vertex data or a node containing no geometry, the values `min` and `max` are both zero.

By default, Scene Kit automatically computes the bounding volumes of nodes and geometries and uses this information to assist in rendering. Setting a new value for this property overrides the default bounding box.

## See Also

### Measuring an Object’s Bounding Volume

var boundingSphere: (center: SCNVector3, radius: Float)

The center point and radius of the object’s bounding sphere.

