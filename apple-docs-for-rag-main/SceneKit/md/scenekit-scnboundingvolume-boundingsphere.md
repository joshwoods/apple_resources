

- SceneKit
- SCNBoundingVolume
-  boundingSphere 

Instance Property

# boundingSphere

The center point and radius of the object’s bounding sphere.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
var boundingSphere: (center: SCNVector3, radius: Float) { get }
```

## Discussion

Scene Kit defines a bounding sphere in the local coordinate space using a center point and a radius. For example, if a node’s bounding sphere has the center point `{3, 1, 4}` and radius `2.0`, all points in the vertex data of node’s geometry (and any geometry attached to its child nodes) lie within `2.0` units of the center point.

The coordinates provided when reading this property are valid only if the object has a volume to be measured. For a geometry containing no vertex data or a node containing no geometry (and whose child nodes, if any, contain no geometry), the values `center` and `radius` are both zero.

## See Also

### Measuring an Object’s Bounding Volume

var boundingBox: (min: SCNVector3, max: SCNVector3)

The minimum and maximum corner points of the object’s bounding box.

