

- SceneKit
- SCNHitTestResult
-  geometryIndex 

Instance Property

# geometryIndex

The index of the geometry element whose surface the search ray intersects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var geometryIndex: Int { get }
```

## Discussion

Every SCNGeometry object contains one or more SCNGeometryElement objects that define how its vertices connect to form a surface. This property provides the index of the geometry element intersecting the search ray. For more information about that geometry element, use the geometry’s element(at:) method.

## See Also

### Retrieving Information About a Hit-Test Result

var node: SCNNode

The node whose geometry intersects the search ray.

var faceIndex: Int

The index of the primitive in the geometry element intersected by the search ray.

var localCoordinates: SCNVector3

The point of intersection between the geometry and the search ray, in the local coordinate system of the node containing the geometry.

var worldCoordinates: SCNVector3

The point of intersection between the geometry and the search ray, in the scene’s world coordinate system.

var localNormal: SCNVector3

The surface normal vector at the point of intersection, in the local coordinate system of the node containing the geometry intersected by the search ray.

var worldNormal: SCNVector3

The surface normal vector at the point of intersection, in the scene’s world coordinate system.

var modelTransform: SCNMatrix4

The world transform matrix of the node containing the intersection.

func textureCoordinates(withMappingChannel: Int) -> CGPoint

Returns the texture coordinates at the point of intersection for the specified texture mapping channel.

