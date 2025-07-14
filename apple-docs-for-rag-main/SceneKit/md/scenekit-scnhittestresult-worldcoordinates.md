

- SceneKit
- SCNHitTestResult
-  worldCoordinates 

Instance Property

# worldCoordinates

The point of intersection between the geometry and the search ray, in the scene’s world coordinate system.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var worldCoordinates: SCNVector3 { get }
```

## See Also

### Retrieving Information About a Hit-Test Result

var node: SCNNode

The node whose geometry intersects the search ray.

var geometryIndex: Int

The index of the geometry element whose surface the search ray intersects.

var faceIndex: Int

The index of the primitive in the geometry element intersected by the search ray.

var localCoordinates: SCNVector3

The point of intersection between the geometry and the search ray, in the local coordinate system of the node containing the geometry.

var localNormal: SCNVector3

The surface normal vector at the point of intersection, in the local coordinate system of the node containing the geometry intersected by the search ray.

var worldNormal: SCNVector3

The surface normal vector at the point of intersection, in the scene’s world coordinate system.

var modelTransform: SCNMatrix4

The world transform matrix of the node containing the intersection.

func textureCoordinates(withMappingChannel: Int) -> CGPoint

Returns the texture coordinates at the point of intersection for the specified texture mapping channel.

